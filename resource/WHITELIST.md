## Requirements

- Provide bank user update whitelist page in management system.(Whitelist is an important part of risk control in finance)
- The user's white list is stored in the **cloud file server** JD Storage, and the index of the whitelist in which the user retrieves the JD Storage is stored in MySQL.
- JD Bill system provides loading whitelist information from cloud server into Redis cache.





## Technology checklist

- Use **H-ui** to add user management whitelist page in management background.
- Use **cloud file server**(JD Storage) to store user whitelist files.
- Use **RPC** to provide whitelist reloading services in JD Bill.
- Use **Redis** to store whitelist information and retrieve Redis directly during risk control.