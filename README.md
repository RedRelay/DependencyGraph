# DependencyGraph

A graph where root nodes are elements (eg. tasks) without any requirements.
Each element (eg. task) has to contains a key used to retrieve elements (eg. tasks) required by other element (eg.task).
This could be used as a tasks scheduler for example.

When you remove a root node, element (eg. task) is considerate as 'finished/done/released', a notification is send to each element which required the removed element.
This notification is used to know if the element, which required the removed element, is now available and could be considered like an element without requirement.
If the element is considered like an element without requirement, it becomes a root node.

Theses sources are originally developed for a Minecraft mod [ForgeCreeperHeal](https://github.com/EyZox/ForgeCreeperHeal) in order to schedule block replacement in a right order.

License : [MIT](https://opensource.org/licenses/MIT)