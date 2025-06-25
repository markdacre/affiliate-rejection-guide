# Lead Rejection Reference Guide
## For Affiliate Partners

---

## Understanding Our Ping & Post Process

Our lead validation operates in two phases:

1. **Ping Phase**: Initial lead information is sent to buyers to gauge interest and receive pricing
2. **Post Phase**: Rigorous validation occurs when the full lead data is submitted

**Important Policy**: Once a lead is rejected during the Post phase, that record becomes inactive in our system. You are free to remarket this lead to other buyers or networks.

---

## Types of Rejections

### RexValidate Rejections
These rejections occur when our internal validation service (RexValidate) identifies data quality issues or requirement mismatches.

| Error Code | Explanation |
|------------|-------------------------|
| **Last Name Does Not Match** | The provided last name does not match property deed records for the submitted address |
| **Not Single Family Residential, Townhouse, Condominium!** | Property type verification failed - address does not correspond to eligible residential property types |
| **Not Single Family Residential!** | Property verification failed - address is not a single-family residence (primarily applies to Roofing leads) |
| **Household Income does not meet requirements** | Submitted household income falls outside the acceptable range for the lead vertical |
| **Home value does not meet requirements** | Property value falls outside the acceptable range for the lead vertical |
| **AI Invalid lead** | Lead content failed our AI validation system (most relevant for MVA leads - comments must be relevant to motor vehicle accidents) |
| **IP to Zip Distance** | Geographical inconsistency detected between IP location and submitted ZIP code |
| **Failed Phone Grade** | Phone number validation failed - number appears to be invalid or disconnected |
| **Not a Residential Address** | Address verification failed - location is not classified as a residential property |
| **Failed Activity Score** | Phone number shows insufficient recent activity (Activity Score indicates 12-month phone usage; scores below 30 suggest disconnected or rarely used numbers) |

### Buyer Rejections
| Error Code | Explanation |
|------------|-------------------------|
| **Not Match / Unmatched** | Lead was successfully submitted to end buyer but rejected based on buyer-specific criteria |

### Technical Issues
| Error Code | Explanation |
|------------|-------------------------|
| **Sub ID is Required** | Missing required subID parameter - check integration specs for "pubsub" or "sub_id" field requirements |

---

## Lead Requirements by Vertical

| Vertical | Home Value Range | Household Income Range |
|----------|------------------|----------------------|
| **Windows** | $80,000 - $5,000,000 | $60,000 - $1,000,000 |
| **Roofing** | $120,000 - $5,000,000 | $75,000 - $1,000,000 |
| **Bath** | $100,000 - $5,000,000 | $65,000 - $1,000,000 |
| **Moving** | N/A | $50,000 - $1,000,000 |
| **MVA** | N/A | Up to $1,000,000 |
| **Debt** | N/A | $35,000 - $1,000,000 |

*Note: For verticals not listed above, filters may not be currently active but are subject to change. We continuously test new fraud prevention services to maintain lead quality.*

---

## Key Reminders

- **Rejected leads are yours to remarket** - Our rejection doesn't prevent you from selling the lead elsewhere
- **Validation is rigorous** - We employ multiple validation services to ensure lead quality for our buyers
- **Requirements evolve** - Filter parameters and validation criteria may change as we optimize our fraud prevention systems
- **Technical support** - For integration issues (missing subID, etc.), refer to your technical specifications or contact support

---

*This guide covers the most common rejection reasons. For additional questions not covered here, please contact your account manager.*
