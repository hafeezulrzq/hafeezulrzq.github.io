# Warren Buffett Financial Ratio Checker

An interactive tool to evaluate companies based on Warren Buffett's investment criteria.

## 🌐 Web Application

The web version is available at: **https://hafeezulrzq.github.io/warren-buffet-financial-ratio-checker**

### Features:
- Interactive checklist interface
- Real-time status indicators as you enter data
- Comprehensive financial ratio analysis
- Investment rating with detailed breakdown
- Beautiful, responsive design matching the Hugo theme

### How to Use:
1. Navigate to the web page
2. Enter the company's financial ratios in each section
3. Check the boxes for consistency indicators where applicable
4. Click "Calculate Investment Rating"
5. Review the detailed analysis and rating

## 📊 Financial Ratios Evaluated

The tool evaluates companies based on the following ratios:

1. **Return on Equity (ROE)** - 15 points
   - Measures how effectively a company uses shareholders' equity
   - Target: Consistently above 15%

2. **Debt-to-Equity Ratio** - 15 points
   - Lower debt means less financial risk
   - Target: Below 0.5

3. **Current Ratio** - 10 points
   - Measures short-term liquidity
   - Target: Above 1.5

4. **Net Profit Margin** - 15 points
   - Shows profitability per dollar of revenue
   - Target: High and consistent margins

5. **Price-to-Earnings (P/E) Ratio** - 10 points
   - Valuation metric
   - Target: Below 20

6. **Price-to-Book (P/B) Ratio** - 10 points
   - Compares market value to book value
   - Target: Below 3

7. **Earnings Growth Rate** - 10 points
   - Consistent earnings growth indicates strong business
   - Target: Steady, predictable growth

8. **Free Cash Flow** - 10 points
   - Positive and growing FCF indicates financial health
   - Target: Positive and growing

**Total Possible Score: 100 points**

## 🎯 Rating System

- **80-100%**: Excellent Investment Opportunity
- **65-79%**: Good Investment Opportunity
- **50-64%**: Moderate Investment Opportunity
- **Below 50%**: Poor Investment Opportunity

## 📝 Notes

- This tool is based on Warren Buffett's general investment principles
- Industry-specific factors may affect the interpretation of certain ratios
- Always conduct thorough due diligence before making investment decisions
- This tool is for educational purposes and should not be considered as financial advice

## 🔧 Deployment

The web version is automatically deployed to GitHub Pages when you push to the repository. The page is built using Hugo:

- Content file: `content/warren-buffet-financial-ratio-checker.md`
- Layout template: `themes/hugo-noir/layouts/_default/warren-buffet-checker.html`

To build and deploy:
1. Run `hugo` to generate the static site
2. The output will be in the `docs/` directory
3. Push to GitHub and it will be available at the URL above

## 📄 License

This project is part of the personal website repository.

