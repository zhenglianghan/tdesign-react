:: BASE_DOC ::

## API

### Guide Props

name | type | default | description | required
-- | -- | -- | -- | --
className | String | - | 类名 | N
style | Object | - | 样式，Typescript：`React.CSSProperties` | N
counter | TElement | - | Typescript：`TNode`。[see more ts definition](https://github.com/Tencent/tdesign-react/blob/develop/src/common.ts) | N
current | Number | 当前步骤，即整个引导的进度。-1 则不展示，用于需要中断展示的场景 | \- | N
defaultCurrent | Number | 当前步骤，即整个引导的进度。-1 则不展示，用于需要中断展示的场景 | uncontrolled property | N
finishButtonProps | Object | { content: '完成', theme: 'primary' } | Typescript：`ButtonProps` | N
hideCounter | Boolean | false | \- | N
hidePrev | Boolean | false | \- | N
hideSkip | Boolean | false | \- | N
highlightPadding | Number | 8 | \- | N
mode | String | popup | options：popup/dialog | N
nextButtonProps | Object | { content: '下一步', theme: 'primary' } | Typescript：`ButtonProps`，[Button API Documents](./button?tab=api)。[see more ts definition](https://github.com/Tencent/tdesign-react/blob/develop/src/guide/type.ts) | N
prevButtonProps | Object | { content: '上一步', theme: 'default' } | Typescript：`ButtonProps` | N
showOverlay | Boolean | true | \- | N
skipButtonProps | Object | { content: '跳过', theme: 'default' } | Typescript：`ButtonProps` | N
steps | Array | - | Typescript：`Array<TdGuideStepProps>` | N
zIndex | Number | 999999 | \- | N
onChange | Function |  | Typescript：`(current: number, context?: { e: MouseEvent,  total: number }) => void`<br/> | N
onFinish | Function |  | Typescript：`(context: { e: MouseEvent, current: number, total: number  }) => void`<br/> | N
onNextStepClick | Function |  | Typescript：`(context: { e: MouseEvent, next: number, current: number, total: number  }) => void`<br/> | N
onPrevStepClick | Function |  | Typescript：`(context: { e: MouseEvent, prev: number, current: number, total: number  }) => void`<br/> | N
onSkip | Function |  | Typescript：`(context: { e: MouseEvent, current: number, total: number  }) => void`<br/> | N

### GuideStep Props

name | type | default | description | required
-- | -- | -- | -- | --
className | String | - | 类名 | N
style | Object | - | 样式，Typescript：`React.CSSProperties` | N
body | TNode | - | Typescript：`string \| TNode`。[see more ts definition](https://github.com/Tencent/tdesign-react/blob/develop/src/common.ts) | N
children | TNode | - | Typescript：`string \| TNode`。[see more ts definition](https://github.com/Tencent/tdesign-react/blob/develop/src/common.ts) | N
content | TElement | - | Typescript：`TNode`。[see more ts definition](https://github.com/Tencent/tdesign-react/blob/develop/src/common.ts) | N
element | String / Function | - | required。Typescript：`AttachNode`。[see more ts definition](https://github.com/Tencent/tdesign-react/blob/develop/src/common.ts) | Y
highlightContent | TElement | - | Typescript：`TNode`。[see more ts definition](https://github.com/Tencent/tdesign-react/blob/develop/src/common.ts) | N
highlightPadding | Number | - | \- | N
mode | String | - | options：popup/dialog | N
nextButtonProps | Object | - | Typescript：`ButtonProps` | N
offset | Array | - | Typescript：`Array<string \| number>` | N
placement | String | 'top' | Typescript：`StepPopupPlacement \| StepDialogPlacement` `type StepPopupPlacement = 'top'\|'left'\|'right'\|'bottom'\|'top-left'\|'top-right'\|'bottom-left'\|'bottom-right'\|'left-top'\|'left-bottom'\|'right-top'\|'right-bottom'` `type StepDialogPlacement = 'top'\|'center' `。[see more ts definition](https://github.com/Tencent/tdesign-react/blob/develop/src/guide/type.ts) | N
prevButtonProps | Object | - | Typescript：`ButtonProps` | N
showOverlay | Boolean | true | \- | N
skipButtonProps | Object | - | Typescript：`ButtonProps` | N
stepOverlayClass | String | - | \- | N
title | String | - | \- | N