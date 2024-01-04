# AituDaniiyarToken

## Usage

This project consists of a simple ERC-20 token named "AITU_Daniyar." The token is implemented using the OpenZeppelin library and includes functionalities to retrieve and display transaction information.

## Demo Screenshots

![Assignment](https://i.postimg.cc/bNKZXFW4/screencapture-remix-ethereum-org-2024-01-04-21-31-22.png)

## Examples

### Retrieve Transaction Information

```solidity
function getTransactionInfo()
    external
    view
    returns (
        address sender,
        address receiver,
        uint256 value
    )
{
    return (msg.sender, address(this), balanceOf(msg.sender));
}
