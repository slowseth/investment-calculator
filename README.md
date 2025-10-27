# Investment Allocation Calculator

A comprehensive, interactive web-based investment calculator that helps users plan their portfolio allocation using low-cost index funds and ETFs. Features detailed growth projections, stress testing, crisis scenarios, and professional PDF/email reports.

## 🌟 Features

### Portfolio Planning
- **Guided Mode**: Pre-built portfolio templates (Simple Two-Fund, S&P 500 Focus, Three-Fund with bonds, etc.)
- **Custom Mode**: Build your own portfolio from 15+ low-cost ETFs (Vanguard, Schwab, Fidelity, iShares)
- **Smart Allocations**: Automatic age-based bond recommendations using Rule of 110
- **Dollar-Cost Averaging**: Model regular contributions (daily, weekly, monthly, quarterly, annually)

### Investment Projections
- **Multiple Scenarios**: Conservative (8%), Expected (10%), Optimistic (12%), and Crisis (2.5%) projections
- **Time Horizons**: Project 1-40 years into the future
- **Visual Charts**: Interactive growth projection and allocation pie charts
- **Detailed Breakdowns**: Dividend income, capital gains, and total returns

### Cost Analysis
- **Expense Ratios**: See blended portfolio costs
- **Fee Impact**: Calculate growth lost to fees over time
- **Financial Advisor Comparison**: Shows cost difference vs. 1% advisor fee (typically saves 96%+ in fees)

### Stress Testing & Crisis Scenarios
- **Historical Crises**: 
  - 2008 Financial Crisis (actual returns)
  - Dot-com Crash 2000-2002 (actual returns)
  - Great Depression style (modeled worst-case)
- **What-If Scenarios**:
  - Small-cap wipeout (-60%)
  - Bond crisis (-20%)
  - International market collapse (-100%)
  - Market armageddon (everything collapses)
- **vs. Cash & Inflation**: Compare invested portfolio vs. keeping money in cash or losing to inflation

### Benchmarking
- **How You Compare**: See your projected portfolio vs. US median and average savings by age group
- **Percentile Ranking**: Understand where you stand (Federal Reserve data)
- **Inflation-Adjusted**: Fair comparisons using today's dollars

### Reports & Exports
- **PDF Reports**: Professional multi-page reports with all calculations and charts
- **Email Reports**: Send detailed text reports via email (EmailJS integration)
- **Shareable**: Easy to save for records or share with financial advisors

## 🚀 Quick Start

### Option 1: Simple Local Setup (No Email)
1. Download `index.html`
2. Open it in any modern web browser
3. Start calculating!

### Option 2: Full Setup (With Email Reports)
1. Download `index.html` and `EMAILJS_SETUP_GUIDE.md`
2. Follow the EmailJS setup guide (takes ~15 minutes)
3. Update the configuration values in `index.html`
4. Deploy to your web hosting or open locally

## 📧 EmailJS Setup (Optional)

The calculator can send professional email reports directly to users and notify you when someone requests a report.

**What you get:**
- ✉️ Users receive professional reports in their inbox
- 📊 You receive user email addresses and all their input data
- 💰 Free tier: 200 emails/month

**Setup Steps:**
1. Sign up at [EmailJS.com](https://www.emailjs.com/)
2. Connect your email service (Gmail recommended)
3. Create 2 email templates (templates provided in setup guide)
4. Update 4 configuration values in `index.html`

See `EMAILJS_SETUP_GUIDE.md` for detailed step-by-step instructions.

## 🔧 Configuration

Open `index.html` and find these lines (around line 118-124):

```javascript
// EmailJS Configuration
const EMAILJS_SERVICE_ID = 'YOUR_SERVICE_ID';
const EMAILJS_TEMPLATE_ID_USER = 'YOUR_USER_TEMPLATE_ID';
const EMAILJS_TEMPLATE_ID_OWNER = 'YOUR_OWNER_TEMPLATE_ID';
const EMAILJS_PUBLIC_KEY = 'emAaG0VJoZvPPV3BA'; // Already set!
const OWNER_EMAIL = 'your-email@example.com';
```

Update these values with your EmailJS credentials.

## 📱 Mobile Responsive

Fully optimized for mobile devices:
- Responsive layouts for all screen sizes
- Touch-friendly inputs and buttons
- Optimized spacing for small screens
- Charts scale appropriately

## 🎨 ETFs Included

**Vanguard:**
- VOO (S&P 500)
- VTI (Total Stock Market)
- VXUS (Total International)
- VB (Small-Cap)
- VWO (Emerging Markets)
- VEA (Developed Markets)
- BND (Total Bond Market)
- BNDX (International Bonds)

**Schwab:**
- SCHX (Large-Cap)
- SCHB (Total Stock Market)
- SCHF (International)
- SCHD (Dividend)

**Fidelity:**
- FXAIX (S&P 500)

**iShares:**
- IVV (S&P 500)
- IEMG (Emerging Markets)

Each ETF includes:
- Real expense ratios
- Current dividend yields
- Tax efficiency ratings
- Turnover rates

## 💡 Use Cases

- **DIY Investors**: Plan your own low-cost index fund portfolio
- **Financial Education**: Learn about asset allocation and compound growth
- **Advisor Comparisons**: See cost difference between self-managing and hiring an advisor
- **Scenario Planning**: Test different allocations and contribution strategies
- **Client Education**: Financial advisors can use to educate clients
- **Blog/Content**: Embed on financial education websites

## 🔐 Privacy & Security

- **No Data Storage**: All calculations happen in the browser
- **No Tracking**: Only Google Analytics for basic page views
- **Email Optional**: EmailJS only activates when user requests a report
- **Open Source**: Full transparency - review all code

## 📊 Technical Details

**Built With:**
- React 18 (via CDN)
- Chart.js 4.4.0
- Tailwind CSS
- jsPDF (PDF generation)
- html2canvas (chart capture)
- EmailJS (email delivery)

**Browser Support:**
- Chrome/Edge (recommended)
- Firefox
- Safari
- Mobile browsers (iOS/Android)

**File Size:** Single HTML file (~150KB)

## 🎯 Calculations & Assumptions

### Growth Projections
- **Conservative**: 8% annual return
- **Expected**: 10% annual return (historical S&P 500 average)
- **Optimistic**: 12% annual return
- **Crisis**: 2.5% annual return

### Fees
- ETF expense ratios deducted from returns
- Financial advisor comparison uses 1% annual fee on assets under management
- Fees compound over time (realistic modeling)

### Inflation
- 3% annual inflation used for real value calculations
- Benchmarks adjusted to today's dollars for fair comparison

### Dollar-Cost Averaging
- Contributions made at beginning of each period
- Growth applied after contribution
- Periods: 252 days, 52 weeks, 12 months, 4 quarters, or 1 year

## 📈 Future Enhancements

Potential features for future versions:
- [ ] Tax loss harvesting calculator
- [ ] Roth vs. Traditional IRA comparison
- [ ] International tax considerations
- [ ] Rebalancing strategies
- [ ] Risk tolerance questionnaire
- [ ] Multi-goal planning
- [ ] Social sharing features
- [ ] Saved portfolios (local storage)

## 🐛 Bug Reports

Found a bug? Please report it by:
1. Checking if it's already been reported
2. Creating a detailed bug report including:
   - Browser and version
   - Steps to reproduce
   - Expected vs. actual behavior
   - Screenshots if applicable

## 📄 License

MIT License - Feel free to use, modify, and distribute.

## ⚠️ Disclaimer

This calculator is for educational purposes only. Projections are based on assumptions and historical averages. Past performance does not guarantee future results. Investment values can fluctuate and you may get back less than invested.

**Not Financial Advice**: This tool does not constitute financial, investment, tax, or legal advice. The information provided is general in nature and may not suit your individual circumstances.

**Consult Professionals**: Always consult with qualified financial advisors, tax professionals, and legal counsel before making investment decisions.

**Tax Implications**: Tax treatment depends on individual circumstances and may change in the future. The calculator provides general estimates only.

**Market Risk**: All investments carry risk. The calculator cannot predict actual market performance or economic conditions.

## 🙏 Acknowledgments

- ETF data sourced from Vanguard, Schwab, Fidelity, and iShares
- Historical crisis data from S&P 500 actual returns
- US savings benchmarks from Federal Reserve Survey of Consumer Finances 2024
- Built with love for DIY investors

## 📞 Support

Questions or need help?
- Review the `EMAILJS_SETUP_GUIDE.md` for email setup
- Check browser console for error messages
- Ensure JavaScript is enabled

---

**Version:** 1.0  
**Last Updated:** October 2025  
**Maintained By:** [Your Name/Organization]

Made with ❤️ for smart investors who want to keep more of their money.
