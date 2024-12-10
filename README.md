

# Scope

*See [scope.txt](https://github.com/code-423n4/2024-12-bakerfi/blob/main/scope.txt)*

### Files in scope


| File   | Logic Contracts | Interfaces | nSLOC | Purpose | Libraries used |
| ------ | --------------- | ---------- | ----- | -----   | ------------ |
| /contracts/core/MultiCommand.sol | 1| **** | 25 | ||
| /contracts/core/VaultRouter.sol | 1| **** | 262 | |@openzeppelin/contracts/interfaces/IERC4626.sol<br>@openzeppelin/contracts/token/ERC20/IERC20.sol<br>@openzeppelin/contracts/token/ERC20/extensions/IERC20Permit.sol|
| /contracts/core/MultiStrategy.sol | 1| **** | 149 | |@openzeppelin/contracts-upgradeable/proxy/utils/Initializable.sol<br>@openzeppelin/contracts/token/ERC20/IERC20.sol<br>@openzeppelin/contracts-upgradeable/access/AccessControlUpgradeable.sol|
| /contracts/libraries/AerodromeLibrary.sol | 1| **** | 50 | |@openzeppelin/contracts/token/ERC20/IERC20.sol<br>@openzeppelin/contracts/token/ERC20/utils/SafeERC20.sol|
| /contracts/libraries/CurveFiLibrary.sol | 1| **** | 71 | |@openzeppelin/contracts/token/ERC20/IERC20.sol<br>@openzeppelin/contracts/token/ERC20/utils/SafeERC20.sol|
| /contracts/libraries/RebaseLibrary.sol | 1| **** | 27 | ||
| /contracts/libraries/MathLibrary.sol | 1| **** | 40 | ||
| /contracts/libraries/UniV2Library.sol | 1| **** | 60 | |@openzeppelin/contracts/token/ERC20/IERC20.sol<br>@openzeppelin/contracts/token/ERC20/utils/SafeERC20.sol|
| /contracts/libraries/UniV3Library.sol | 1| **** | 48 | |@openzeppelin/contracts/token/ERC20/IERC20.sol<br>@openzeppelin/contracts/token/ERC20/utils/SafeERC20.sol|
| /contracts/core/router/Commands.sol | 1| **** | 48 | ||
| **Totals** | **10** | **** | **780** | | |

### Files out of scope

*See [out_of_scope.txt](https://github.com/code-423n4/2024-12-bakerfi/blob/main/out_of_scope.txt)*

| File         |
| ------------ |
| ./contracts/core/Constants.sol |
| ./contracts/core/EmptySlot.sol |
| ./contracts/core/GovernableOwnable.sol |
| ./contracts/core/MultiStrategyVault.sol |
| ./contracts/core/Vault.sol |
| ./contracts/core/VaultRegistry.sol |
| ./contracts/core/VaultSettings.sol |
| ./contracts/core/flashloan/BalancerFlashLender.sol |
| ./contracts/core/governance/BKR.sol |
| ./contracts/core/governance/BakerFiGovernor.sol |
| ./contracts/core/governance/Timelock.sol |
| ./contracts/core/hooks/UseAAVEv3.sol |
| ./contracts/core/hooks/UseFlashLender.sol |
| ./contracts/core/hooks/UseIERC20.sol |
| ./contracts/core/hooks/UseIERC4626.sol |
| ./contracts/core/hooks/UseLeverage.sol |
| ./contracts/core/hooks/UseOracle.sol |
| ./contracts/core/hooks/UsePermitTransfers.sol |
| ./contracts/core/hooks/UseStETH.sol |
| ./contracts/core/hooks/UseStrategy.sol |
| ./contracts/core/hooks/UseTokenActions.sol |
| ./contracts/core/hooks/UseUniQuoter.sol |
| ./contracts/core/hooks/UseWETH.sol |
| ./contracts/core/hooks/UseWstETH.sol |
| ./contracts/core/hooks/swappers/UseAeroSwapper.sol |
| ./contracts/core/hooks/swappers/UseCurveSwapper.sol |
| ./contracts/core/hooks/swappers/UseUniV2Swapper.sol |
| ./contracts/core/hooks/swappers/UseUniV3Swapper.sol |
| ./contracts/core/hooks/swappers/UseUnifiedSwapper.sol |
| ./contracts/core/strategies/StrategyAeroSwapAnd.sol |
| ./contracts/core/strategies/StrategyCurveSwapAnd.sol |
| ./contracts/core/strategies/StrategyLeverage.sol |
| ./contracts/core/strategies/StrategyLeverageAAVEv3.sol |
| ./contracts/core/strategies/StrategyLeverageMorphoBlue.sol |
| ./contracts/core/strategies/StrategyLeverageSettings.sol |
| ./contracts/core/strategies/StrategyPark.sol |
| ./contracts/core/strategies/StrategySettings.sol |
| ./contracts/core/strategies/StrategySupplyAAVEv3.sol |
| ./contracts/core/strategies/StrategySwapAnd.sol |
| ./contracts/core/strategies/StrategyUniV2SwapAnd.sol |
| ./contracts/core/strategies/StrategyUniV3SwapAnd.sol |
| ./contracts/interfaces/aave/v3/DataTypes.sol |
| ./contracts/interfaces/aave/v3/IPoolAddressesProvider.sol |
| ./contracts/interfaces/aave/v3/IPoolV3.sol |
| ./contracts/interfaces/aerodrome/ISwapRouter.sol |
| ./contracts/interfaces/balancer/IFlashLoan.sol |
| ./contracts/interfaces/balancer/IProtocolFeesCollector.sol |
| ./contracts/interfaces/balancer/IVault.sol |
| ./contracts/interfaces/chainlink/IChainlinkAggregator.sol |
| ./contracts/interfaces/core/IOracle.sol |
| ./contracts/interfaces/core/IStrategy.sol |
| ./contracts/interfaces/core/IStrategyLeverage.sol |
| ./contracts/interfaces/core/IStrategySettings.sol |
| ./contracts/interfaces/core/ISwapHandler.sol |
| ./contracts/interfaces/core/IVault.sol |
| ./contracts/interfaces/core/IVaultRegistry.sol |
| ./contracts/interfaces/core/IVaultSettings.sol |
| ./contracts/interfaces/curve/ICurvePool.sol |
| ./contracts/interfaces/curve/ICurveRouterNG.sol |
| ./contracts/interfaces/lido/IStETH.sol |
| ./contracts/interfaces/lido/IWStETH.sol |
| ./contracts/interfaces/pyth/IPyth.sol |
| ./contracts/interfaces/pyth/IPythEvents.sol |
| ./contracts/interfaces/pyth/PythStructs.sol |
| ./contracts/interfaces/tokens/IWETH.sol |
| ./contracts/interfaces/uniswap/v2/IUniswapV2Router01.sol |
| ./contracts/interfaces/uniswap/v2/IUniswapV2Router02.sol |
| ./contracts/interfaces/uniswap/v3/IQuoterV2.sol |
| ./contracts/interfaces/uniswap/v3/IUniswapV3Pool.sol |
| ./contracts/interfaces/uniswap/v3/IV3SwapRouter.sol |
| ./contracts/mocks/AAVE3PoolMock.sol |
| ./contracts/mocks/BalancerVaultMock.sol |
| ./contracts/mocks/BorrowerAttacker.sol |
| ./contracts/mocks/ChainLinkAggregatorMock.sol |
| ./contracts/mocks/CommandMock.sol |
| ./contracts/mocks/ERC20Mock.sol |
| ./contracts/mocks/ERC3156FlashBorrowerMock.sol |
| ./contracts/mocks/ERC3156FlashLender.sol |
| ./contracts/mocks/ERC4626VaultMock.sol |
| ./contracts/mocks/MathLibraryWrapper.sol |
| ./contracts/mocks/OracleMock.sol |
| ./contracts/mocks/PythMock.sol |
| ./contracts/mocks/QuoterV2Mock.sol |
| ./contracts/mocks/StrategyLeverageSettingsMock.sol |
| ./contracts/mocks/StrategyMock.sol |
| ./contracts/mocks/UniV3RouterMock.sol |
| ./contracts/mocks/VaultRouterMock.sol |
| ./contracts/mocks/WETH.sol |
| ./contracts/mocks/WstETH.sol |
| ./contracts/oracles/ChainLinkExRateOracle.sol |
| ./contracts/oracles/ChainLinkOracle.sol |
| ./contracts/oracles/CustomExRateOracle.sol |
| ./contracts/oracles/ExRateOracle.sol |
| ./contracts/oracles/PythOracle.sol |
| ./contracts/oracles/RatioOracle.sol |
| ./contracts/proxy/BakerFiProxy.sol |
| ./contracts/proxy/BakerFiProxyAdmin.sol |
| ./contracts/tests/BoringRebaseTest.sol |
| ./contracts/tests/LeverageTest.sol |
| ./contracts/tests/RebaseLibraryTest.sol |
| Totals: 100 |

