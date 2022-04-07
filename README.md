# decision-kit

Tree-based library, with branching criteria based on Gini impurity. At the moment only a classification decision tree and a RandomForest based on it are implemented.

```python
from utils.helper import accuracy
from tree._tree import DecisionTree

classifier = DecisionTree()
classifier.grow(header, xtrain, ytrain)
predicted_val = classifier.predict(header, xtest)
acc = accuracy(predicted_val, ytest)
print(acc)
```