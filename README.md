## Hi there 👋
# Crypto Coders | آموزش تخصصی برنامه‌نویسی بلاکچین و قراردادهای هوشمند

به گیت‌هاب رسمی **Crypto Coders** خوش آمدید!
این مجموعه شامل سورس‌کد کامل پروژه‌های عملی Web3، قراردادهای هوشمند **Solidity** و کدهای آموزشی منتشرشده در کانال یوتیوب **Crypto Coders** (`@Crypto_Coders`) است.

- **کانال یوتیوب:** Crypto Coders (`@Crypto_Coders`)
- **تلگرام:** `@CryptoCoders_tel`
- **حوزه تخصصی:** Solidity • Smart Contracts • Ethereum & EVM • DeFi & Web3 Security

## ۱. پروژه‌های کاربردی و واقعی قرارداد هوشمند (Real-World Smart Contracts)

این ریپازیتوری‌ها شامل پیاده‌سازی کامل پروژه‌های واقعی بلاکچین و دیفای به زبان `Solidity ^0.8.20 / ^0.8.24` همراه با الگوهای امنیتی استاندارد (مانند جلوگیری از Reentrancy، الگوی Pull Payment و مدیریت خطاهای سفارشی) هستند:

| ردیف | نام ریپازیتوری | قرارداد(ها) | توضیحات پروژه |
| :--- | :--- | :--- | :--- |
| ۱ | `Auctions` | `DutchAuction`, `DecentralizedAuction`, `SealedBidAuction`, `VickreyAuction` | مجموعه ۴ قرارداد هوشمند مزایده (انگلیسی، هلندی، پاکت‌بسته اول‌قیمت و مزایده ویکری دوم‌قیمت با مکانیزم Commit-Reveal) |
| ۲ | `VestingWalletETH` | `VestingWallet` | کیف پول زمان‌بندی و قفل دارایی (Vesting Wallet) بر پایه Native ETH با دوره تنفس (Cliff)، آزادسازی خطی و قابلیت لغو توسط مالک |
| ۳ | `StakingRewards` | `NativeStakingRewards` | سیستم استیکینگ Native ETH و توزیع پاداش لحظه‌ای بر اساس زمان با الگوریتم شاخص تجمعی `rewardPerToken` |
| ۴ | `DAOvoting` | `DAOVotingSystem` | سیستم رأی‌گیری سازمان مستقل غیرمتمرکز (DAO) با مدیریت اعضا، پروپوزال‌ها، حد نصاب (`quorum`) و سه گزینه رأی (موافق، مخالف، ممتنع) |
| ۵ | `MultiSignatureWallet` | `MultiSignatureWallet` | کیف پول چندامضایی (Multi-Sig Wallet) برای ثبت، تأیید، لغو تأیید و اجرای تراکنش‌های گروهی با حد نصاب امضای مالکان |
| ۶ | `Escrow` | `EscrowSystemPayment` | سیستم پرداخت امانی (Escrow) سه‌جانبه بین کارفرما (`client`)، مجری (`customer`) و داور (`refree`) همراه با مدیریت اختلاف و مهلت زمانی |
| ۷ | `Crowdfunding` | `CrowdfundingPlatform` | پلتفرم جذب سرمایه جمعی (Crowdfunding) با بررسی و تأیید کمپین توسط ادمین، کارمزد ۲٪ پلتفرم و استرداد وجه کمپین‌های ناموفق |
| ۸ | `cryptoBank` | `ICryptoBank`, `BankBase`, `CryptoBank` | پروژه بانک کریپتویی با معماری ماژولار (Interface و ارث‌بری)، کارمزد ۲ درصدی، مدیریت وضعیت بانک و ثبت تاریخچه سپرده‌ها |
| ۹ | `Auction` | — | ریپازیتوری معرفی و ارجاع به مجموعه پروژه‌های مزایده در ریپازیتوری اصلی `Auctions` |

## ۲. دوره جامع آموزش مقدماتی تا پیشرفته سالیدیتی (Solidity Fundamentals)

این ریپازیتوری‌ها به ترتیب سرفصل‌های آموزشی، مفاهیم پایه تا پیشرفته زبان **Solidity** را به همراه مثال‌های کاربردی پوشش می‌دهند:

| ردیف | نام ریپازیتوری | فایل‌ها و قراردادها | مبحث آموزشی |
| :--- | :--- | :--- | :--- |
| ۱ | `First-Solidity-Coding-Touch` | `StartSolidity.sol` (`NumberGame`) | آشنایی با ساختار اولین قرارداد هوشمند، سازنده (`constructor`)، توابع و مودیفایرهای پایه |
| ۲ | `variables-1` | `BaseVariables.sol` (`BaseVariables`) | انواع داده پایه (`bool`, `uint`, `int`, `address`, `bytes`, `string`)، ثوابت (`constant`, `immutable`) و سطوح دسترسی متغیرها |
| ۳ | `Base-Functions` | `BaseFunctions.sol` (`FunctionExamples`) | ساختار توابع پایه، سطوح دسترسی (`public`, `external`) و انواع توابع (`view`, `pure`, `payable`) |
| ۴ | `Global-Variables` | `Globalvariable.sol`, `A.sol`, `B.sol` | متغیرهای سراسری بلاک، تراکنش و پیام (`msg.sender`, `msg.value`, `block.timestamp`, `tx.origin`) و تفاوت عملی `msg.sender` با `tx.origin` |
| ۵ | `ControlStructures` | `ControlStructures.sol` (`ControlStructures`) | ساختارهای کنترلی و شرطی (`if / else`) و پیمایش با حلقه‌های `for` و `while` |
| ۶ | `Mapping-Enum-Struct` | `Enum.sol`, `Mapping.sol`, `NestedMapping.sol`, `Struct.sol`, `OrderingSystem.sol` | ساختارهای داده پیشرفته (`enum`, `struct`, `mapping`, `Nested Mapping`) و پروژه ترکیبی سیستم سفارش‌گیری |
| ۷ | `ERROR-MODIFIRE` | `ErrorHandlingAndModifiers.sol` | مدیریت خطا با `require`، `revert` و خطاهای سفارشی (`Custom Error`) بهینه از نظر گس همراه با `modifier` |
| ۸ | `Events` | `Event.sol` (`EventExample`) | تعریف رویدادها (`event`)، پارامترهای `indexed` و ثبت لاگ روی بلاکچین با `emit` |
| ۹ | `Recive-Send-ETH` | `SpecialReceivesFunctions.sol`, `TransfersFunctions.sol` | دریافت مستقیم اتر (`receive` و `fallback`) و مقایسه سه روش ارسال اتر (`transfer`, `send` و `call`) |
| ۱۰ | `Inheritance-Interface` | `IAnimal.sol`, `Animal.sol`, `Dog.sol`, `Inheritance.sol`, `Interface.sol` | ارث‌بری تک‌سطحی و چندگانه (`is`, `virtual`, `override`, `super`)، تعریف `interface` و استفاده از `import` |
| ۱۱ | `Deploy-test` | `DeployTest.sol` (`AdvancedStorage`) | تمرین کامپایل، دیپلوی و تعامل با قرارداد هوشمند شامل متغیرهای خصوصی، رویدادها و انتقال مالکیت |

## ۳. نحوه اجرا و تست کدها

1. وارد محیط **Remix IDE** شوید یا از فریم‌ورک‌های **Hardhat / Foundry** استفاده کنید.
2. فایل `.sol` مورد نظر را از ریپازیتوری مربوطه باز کرده و با نسخه کامپایلر درج‌شده در بالای فایل (`^0.8.0` تا `^0.8.24`) کامپایل کنید.
3. در بخش **Deploy & Run Transactions** قرارداد را دیپلوی کرده و توابع آن را طبق توضیحات `README.md` هر ریپازیتوری تست کنید.
<!--
**CryptoCodersGit/CryptoCodersGit** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
