### Task
Markdown file 2: Why does the `SafeERC20` program exist and when should it be used?

### Answer
In the `ERC20` standard, transfer and transferFrom return a boolean and do not revert. 
`SafeERC20` is a set of wrappers around `ERC20` operations that reverts when the return value is false or no value at all.

You should use the `SafeERC20` library when your contract interacts with the `ERC20` token.