# Simple-Mapping-9
Simple Mapping.sol
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract SimpleMapping {
    mapping(address => uint) public balances;

    function setBalance(uint _amount) public {
        balances[msg.sender] = _amount;
    }
}
