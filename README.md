# В чем разница между структурными и атрибутивными директивами?

Структурные директивы нужны для изминения структцры DOM за счет удаления или добавления элементов.
Атрибутивные директивы используются для изменения внешнего вида или поведения элемента DOM.
Атрибутивные директивы меняют поведение элемента, к которому они применяются. Например, директива ngClass позволяет установить для элемента класс CSS. При этом сама директива применяется к элементу в виде атрибута.

# Что такое trackByFn?

trackByFn используется при перебора массива директивой *ngFor. trackByFn используется для оптимизации производительности. А если использовать trackBy Angular будет изменять DOM только для этого конкретного элемента. Если использовать trackBy angulat будет изменять dom дерево для конкретного отличного элемента не обновляя все DOM-дерево.

# В чем разница между ngIf и display: none?

Директива ngIf полностью удаляет элеиент со страницы и DOM-дерева(если условие его отображения не потвердилось). При использовании display: none элемент скрывается со страницы но не удаляется из DOM. При использовании display: none елемент просто скрывается, не исчезая из DOM-дерева. ngIf лучше для оптимизации и производительности.

# ПОбъясните десятичную трубу

Decimal pipe позволяют форматировать отображаемые значения, именно числа,number. В качестве параметра принимает формат числа в виде шаблона: {{ value | number [ : digitsInfo [ : locale ] ] }} value: само выводимое значение digitsInfo: строка в формате "minIntegerDigits.minFractionDigits-maxFractionDigits", где minIntegerDigits — минимальное количество цифр в целой части minFractionDigits — минимальное количество цифр в дробной части maxFractionDigits — максимальное количество цифр в дробной части locale: код применяемой культуры
