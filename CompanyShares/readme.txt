
Initial folder setup

Description:

Blockchain code in solidity to build a share structure for a company 

Compatability for NRC20 and BEP20 

Instructions:

Code can be found at: https://github.com/ShaneCalderDuckyA50/CacheDEFIProject/blob/main/CompanyShares/CompanyShares.sol

Lines 4 to 13 should be eddited to include company information 
Code example here:

// CompanyName - (Place company Name here)
// Founders - 
// Company Location - Country - City 
// Type of Company Corporation etc.
// Public or private company  
// Class of shares 
// Company holding sale of shares or underwriter (if required)
// Date for financial statements or year end
// Website: 
// Contact email or phone number 

Lines 362 - 365 total token supply can be changed (set at 10,000 shares), change name to company name and symbol. Set to 2 decimal points. 

Code example here: 
  constructor() public {
    _name = "Company Name"; 
    _symbol = "COMPANY";
    _decimals = 2;
    _totalSupply = 10000 * 10 **2;
    _balances[msg.sender] = _totalSupply;

    emit Transfer(address(0), msg.sender, _totalSupply);
  }
  
  Notes: 
  Can be complied with no errors. 
  Code is in draft form first revission. 

