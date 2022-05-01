

# InlineResponse2001

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**state** | **String** | 响应状态分为：-1,0,1 分别代表响应错误、响应提示、响应成功 | 
**msg** | **String** | 响应状态为-1时该值为错误信息。响应状态为0时，该值为响应提示信息。响应状态为1时该值为空字符串 | 
**phone** | **String** |  | 
**virifycodeid** | **String** | 验证码图片的ID值 | 
**virifyimage** | **String** | data:image/png;base64 | 
**confluxaddress** | **String** | 树图区块链地址 | 
**ethaddress** | **String** | 以太坊、Arbitrum、polygon、BSC等EVM链地址 | 
**token** | **String** | 用户登录识别令牌，用于后续多个函数的交互，作为输入参数 | 



