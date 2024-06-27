// SPDX-License-Identifier: UNLICENSED
pragma solidity ^0.8.17;

// @title BasicMath
// @notice This contract is used to test the overflow detection
// @author NelsonRodMar
contract BasicMath {
    constructor() {}

    // @notice This function return the sum of the two number and a boold true if overflow otherwise false
    // @param _a The first number
    // @param _b The second number
    // @return sum The sum of the two number
    // @return error True if overflow otherwise false
    function adder(uint256 _a, uint256 _b) public pure returns (uint256 sum, bool error) {
        unchecked {
            if (_a + _b >= _a) {
                sum = _a + _b;
                error = false;
            } else {
                sum = 0;
                error = true;
            }
        }
    }

    // @notice This function return the difference of the two number and a boold true if overflow otherwise false
    // @param _a The first number
    // @param _b The second number
    // @return difference The difference of the two number
    // @return error True if overflow otherwise false
    function subtractor(uint256 _a, uint256 _b) public pure returns (uint256 difference, bool error) {
        unchecked {
            if (_a - _b <= _a) {
                difference = _a - _b;
                error = false;
            } else {
                difference = 0;
                error = true;
            }
        }
    }
}
