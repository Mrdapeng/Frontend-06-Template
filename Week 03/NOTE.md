学习笔记

reg.exec(str)匹配成功后，调用exec()返回一个数组(附加属性index和input)，并更新正则表达式对象的lastIndex属性。如果完全匹配，则文本作为数组中的第一项返回，从第二项开始的每一项都对应于正则表达式中括号内的文本。如果匹配失败，exec()方法返回null并将lastIndex重置为0。

注意：不要在while表达式中放入正则表达式字元（或RegExp构造函数）。由于 lastIndex 属性在每次迭代时都会被重置，所以如果匹配的话会导致死循环。确保'g'标签用于全局匹配，否则会引起死循环。

get：exec()类似于string.matchAll(reg)，是matchAll的迭代器 get：match()在使用g标志时返回成功匹配的文本，在不使用g时返回匹配的文本和捕获组。

LL AST 
词汇分析
我们通过规律匹配得到相应的词，通过生成函数得到数组结构。

语法分析
Expression: AdditveExpression和Expression的组合 AdditveExpression。AdditveExpression和MultiplicaliveExpression的组合 MultiplicalExpression: 乘法表达式和数字的组合。

