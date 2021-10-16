# Financial-Ratios-API
Tradefeeds is a provider of real-time REST JSON API for financial ratios data. Our <a href=""> Financial Ratios Database</a> contains 76 types of financial ratios used frequently by analysts and investors when evaluating companies. The data is organized according to the six main groups of financial ratios: liquidity ratios, solvency ratios (also known as leverage ratios), turnover ratios (also known as leverage ratios), profitability ratios and market value measures, as well as other uncategorized ratios. We use mathematical formulas to calculate the financial ratios in Tradefeeds API database. The system uses the financial information disclosed in the annual or quarterly reports of companies during a particular year or a quarter. Customers should select a company, a financial reporting period and formulas for which they want to obtain data on financial ratios.

Our customers are diverse starting from developers, investors, traders, creditors to universities and research centes. Developers would build mobile and web applications with the help of financial ratios data API. Compared to them, financial analysts, investors, traders, universities and research centers use the API for financial ratios to perform company valuation. 

Tradefeeds subscription packages are developed in such a way to serve all customers' needs. For the moment, there is no free trial provided. In case that you are a researcher or a student, we could negotiate a free trial. <a href="https://tradefeeds.com/pricing-subscription-plans/" rel="nofollow"> Sign up for an API key</a> and we work out your case.

<h2><a id="user-content-api-features" class="anchor" href="https://github.com/Tradefeeds-Financial-data-API/Company-information-API#api-features" aria-hidden="true"></a>API Features</h2>

<li><strong>Liquidity Ratios</strong></li>
<li><strong>Solvency Ratios</strong></li>
<li><strong>Turonver Ratios</strong></li>
<li><strong>Profitability Ratios</strong></li>
<li><strong>Market Value Measures</strong></li>
<li><strong>Uncategorized Ratios</strong></li>

<h2><a id="user-content-ways-to-access-company-data" class="anchor" href="https://github.com/Tradefeeds-Financial-data-API/Company-information-API#ways-to-access-financial-ratios-data" aria-hidden="true"></a>Ways to access financial ratios data</h2>
<ul>
 	<li><strong>JSON REST API</strong></li>
 	<li><strong>Excel CSV download</strong></li>
 	<li><strong>PDF reports</strong></li>
 	<li><strong>Email link</strong></li>
</ul>

<h2>Documentation</h2>

Our <a href="https://tradefeeds.com/documentation" rel="nofollow">documentation</a> includes input API filtering parameters, output response objects with explanation of their meaning. Clear request and response examples are given on the documentation page. Furthermore, we provide SDKs for Javascript, JQuery, VueJS, Angular, JAVA, PHP, NodeJS, Python, Go, Ruby, C#, R, Strest, Rust, Swift and Scala

<h2>Request and response examples</h2>

<strong>Example 1: You search for all financial ratios of Apple Inc.</strong> 

<a href="https://tradefeeds.com/api-documentation/">https://tradefeeds.com/api/v1/financialratios?key=YOUR-KEY&stock_ticker_symbol=aapl</a>

    "status": {
        "message": "Success"
    },
    "results": [
        {
        "basics": {
            "name": "Apple Inc",
            "stock_ticker_symbol": "AAPL"
            "isin_identifier": "US0378331005"
            "exchange": "nasdaq"
            "industry": "technology"
            "sector": "consumer electronics"
        },
        "output": {
           "currentRatio": "1.3636044481554577"
            "quickRatio": "1.2181949294064065"
            "cashRatio": "0.36071049035979963"
            "daysOfSalesOutstanding": "49.78753437881355"
            "daysOfInventoryOutstanding": "8.741883356235881"
            "operatingCycle": "58.52941773504943"
            "daysOfPayablesOutstanding": "91.04818971567418"
            "cashConversionCycle": "-32.518771980624756"
            "grossProfitMargin": "0.38233247727810865"
            "operatingProfitMargin": "0.24147314354406862"
            "pretaxProfitMargin": "0.24439830246070343"
            "netProfitMargin": "0.20913611278072236"
            "effectiveTaxRate":" 0.14428164731484103"
            "returnOnAssets": "0.1772557180259843"
            "returnOnEquity": "0.8786635853012749"
            "returnOnCapitalEmployed": "0.3033831282952548"
            "netIncomePerEBT": "0.855718352685159"
            "ebtPerEbit": "1.0121138064204682"
            "ebitPerRevenue": "0.24147314354406862"
            "debtRatio": "0.7982666847799239"
            "debtEquityRatio": "3.957039440456695"
            "longTermDebtToCapitalization": "0.6016060388034584"
            "totalDebtToCapitalization": "0.6324623822247223"
            "interestCoverage": "23.07274625826662"
            "cashFlowToDebtRatio": "0.7175104059198122"
            "companyEquityMultiplier": "4.957039440456695"
            "receivablesTurnover": "7.331152356789959"
            "payablesTurnover": "4.008866086627577"
            "inventoryTurnover": "41.75301649839941"
            "fixedAssetTurnover": "7.466545177609748"
            "assetTurnover": "0.8475615027416885"
            "operatingCashFlowPerShare": "4.649230448454163"
            "freeCashFlowPerShare": "4.2280138811865"
        }
 
        
<strong>Example 2: You search for data on the current ratios, quick ratios and cash ratios of Apple Inc. Microsoft and Dell Technologies Inc.</strong>

<a href="https://tradefeeds.com/api-documentation/">https://tradefeeds.com/api/v1/financialratios?key=YOUR-KEY&stock_ticker_symbol=aapl,msft,dell&financial-ratio=current_ratio,quick_ratio,cash_ratio</a>

    "status": {
        "message": "Success"
    },
    "results": [
        {
        "basics": {
            "name": "Apple Inc",
            "stock_ticker_symbol": "AAPL"
            "isin_identifier": "US0378331005"
            "exchange": "nasdaq"
            "industry": "technology"
            "sector": "consumer electronics"
        },
        "output": {
           "current_ratio": "1.3636044481554577"
            "quick_ratio": "1.2181949294064065"
            "cash_ratio": "0.36071049035979963"
        },
        "basics": {
            "name": "Microsoft Corporation",
            "stock_ticker_symbol": "MSFT"
            "isin_identifier": "US5949181045"
            "exchange": "nasdaq"
            "industry": "technology"
            "sector": "consumer electronics"
        },
        "output": {
           "current_ratio": "1.8155457736360444"
            "quick_ratio": "1.2940640652181949"
            "cash_ratio": "0.49035979963360710"
        },
        "basics": {
            "name": "Dell Technologies Inc",
            "stock_ticker_symbol": "DELL"
            "isin_identifier": "US24703L2025"
            "exchange": "NYSE"
            "industry": "technology"
            "sector": "consumer electronics"
        },
        "output": {
           "current_ratio": "1.4815545773636044"
            "quick_ratio": "1.2940640218194965"
            "cash_ratio": "0.35979963360710490"
        },


<h2>Customer support</h2>
In case that you encounter a data issue or you want to have more features added to the API, please contact us at support@tradefeeds.com.

<h2>Legal</h2>
<p> The use of Tradefeeds proprietary data and API database is subject to the&nbsp;<a href="https://tradefeeds.com/terms-and-conditions-on-data/">Tradefeeds Terms &amp; Conditions.</a></p>

