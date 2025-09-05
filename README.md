# Google-calendar-Create-event-
Google Calendar Create Event MCP tool that lets your AI voice agents schedule events via a simple URL endpoint. Seamlessly connect to Google Calendar and create events directly from user requests


WATCH THIS FOR FULL INTEGRATION👇

[](https://youtu.be/hNytZ4DPlus?si=NhbDBRlNO_SdcN_C)](https://youtu.be/hNytZ4DPlus?si=NhbDBRlNO_SdcN_C)

# 📅 Google Calendar Event Creation - Complete User Guide

🤖 **AI Voice Agent Integration** | 📅 **Google Calendar API** | 🔐 **Secure Credentials** | ⚡ **Retell.ai Ready**

Create calendar events in Google Calendar through voice commands using Retell.ai or any MCP-compatible AI agent. Each business owner configures their credentials once for unlimited automated bookings.

---

## **🤖 AI Agent Optimization for Business Owners**

### **Maximize Your Booking Success Rate with Smart AI Configuration**

This section helps business owners configure their AI agents to create seamless, professional booking experiences that gather all necessary information while providing excellent customer service.

---

## **🎯 Critical AI Agent Configuration Areas**

### **1. 📅 Time & Date Management**

#### **✅ Essential AI Prompts:**
```
"Always confirm the current date and time before scheduling. Today is [CURRENT_DATE]. 
Our timezone is [YOUR_TIMEZONE]. When customers say 'tomorrow', 'next week', 
or 'Monday', calculate the exact date and confirm it with them."
```

#### **⚠️ Common Time Issues to Address:**
- **Relative dates**: "tomorrow", "next week", "Monday"
- **Time zone confusion**: Customer vs. business timezone
- **AM/PM clarification**: "2 o'clock" could be 2 AM or 2 PM
- **Business hours**: Don't book outside operating hours

#### **🔧 Recommended AI Instructions:**
```
"Business Hours: [YOUR HOURS, e.g., Monday-Friday 9 AM - 6 PM EST]
- Always convert customer requests to exact dates and times
- Confirm 'I have you down for [DAY], [DATE] at [TIME]'
- If customer says 'morning', ask 'What time in the morning works best?'
- Never book appointments outside business hours without explicit approval"
```

---

### **2. 📝 Default Event Information & Customer Parameters**

#### **✅ Configure Customer Data Collection:**
```
"Customer information parameters (all optional - configure as needed):
- customerName: Customer's full name (auto-added to event title)
- customerPhone: Phone number (auto-added to description) 
- customerEmail: Email address (auto-added as attendee)
- serviceType: Type of service (auto-added to event title)
- specialNotes: Special requests (auto-added to description)"
```

#### **✅ AI Prompt Examples for Different Data Collection Levels:**

**Full Data Collection:**
```
"Always collect and send these parameters:
- customerName: Get full name
- customerPhone: Ask for phone number  
- customerEmail: Get email for calendar invite
- serviceType: Ask what service they need
- specialNotes: Ask for any special requests"
```

**Minimal Data Collection:**
```
"Only collect essential information:
- customerName: Get customer name
- serviceType: Ask what service they need
- Do not require phone number or email address"
```

**Privacy-Focused Collection:**
```
"Respect customer privacy:
- customerName: Get first name only
- serviceType: Ask what service they need
- Do not collect phone, email, or personal notes"
```

#### **✅ Pre-Configure These Details:**
```
"Default meeting information to include:
- Meeting Title Format: '[SERVICE_TYPE] - [CUSTOMER_NAME]'
- Default Duration: [30/60 minutes]
- Default Location: '[YOUR_ADDRESS or 'Phone Call' or 'Video Call']'
- Default Description Template: 'Service: [TYPE]\nCustomer: [NAME]\nPhone: [PHONE]\nNotes: [SPECIAL_REQUESTS]'"
```

#### **📋 Business-Specific Examples:**

**Dental Office:**
```
"Default appointment titles: 'Dental [APPOINTMENT_TYPE] - [PATIENT_NAME]'
Default duration: 60 minutes for cleanings, 30 minutes for consultations
Always include: Patient phone number, insurance information if provided"
```

**Law Firm:**
```
"Default consultation titles: 'Legal Consultation - [CLIENT_NAME]'
Default duration: 45 minutes
Always include: Case type, urgency level, preferred contact method"
```

**Hair Salon:**
```
"Default appointment titles: '[SERVICE] Appointment - [CLIENT_NAME]'
Services: Haircut (60 min), Color (120 min), Highlights (180 min)
Always ask: Previous stylist preference, special requests"
```

---

### **💬 Customer Information Collection Options**

The actor supports flexible customer data collection. Business owners can configure their AI agent to collect as much or as little customer information as desired.

#### **✅ Available Customer Parameters:**
- **`customerName`** - Full name (auto-generates event titles)
- **`customerPhone`** - Phone number (auto-added to description)
- **`customerEmail`** - Email address (auto-added as calendar attendee)
- **`serviceType`** - Service requested (auto-added to event title)
- **`specialNotes`** - Special requests (auto-added to description)

#### **🎯 Business Configuration Examples:**

**Medical Practice (Full Information):**
```
AI Prompt: "Always collect: customerName, customerPhone, customerEmail, serviceType. 
Ask: 'What's your full name?', 'Phone number?', 'Email for appointment confirmation?', 'What type of appointment?'"
```

**Restaurant (Minimal Information):**
```
AI Prompt: "Only collect: customerName, specialNotes for party size and dietary restrictions. 
Do not require phone or email. Ask: 'Name for the reservation?', 'Any dietary restrictions?'"
```

**Hair Salon (Selective Information):**
```
AI Prompt: "Collect: customerName, customerPhone, serviceType. 
Skip email collection. Ask: 'Your name?', 'Phone number?', 'What service would you like?'"
```

#### **✅ Essential Information to Collect:**
```
"Always gather these details before booking:
1. Full name (first and last)
2. Phone number 
3. Email address (for calendar invite)
4. Service type requested
5. Any special needs or requests
6. Preferred contact method for reminders"
```

#### **🎯 Smart Questioning Flow:**
```
"Information gathering script:
1. 'What type of [service] are you looking for?'
2. 'What's the best phone number to reach you?'
3. 'And your email for the calendar invite?'
4. 'Any special requests or things I should note?'
5. 'How would you prefer we contact you for any updates?'"
```

#### **⚠️ What NOT to Over-Ask:**
- Don't ask for unnecessary personal details
- Don't require information you won't use
- Don't ask the same question multiple ways
- Don't interrupt the flow with too many questions

---

### **4. 🔄 Confirmation & Validation**

#### **✅ Always Confirm These Details:**
```
"Before finalizing any booking, confirm:
'Let me confirm your appointment:
- Service: [SERVICE_TYPE]
- Date & Time: [DAY], [DATE] at [TIME]
- Duration: [X] minutes
- Location: [LOCATION]
- Name: [FULL_NAME]
- Phone: [PHONE_NUMBER]
- Email: [EMAIL]

Does this look correct?'"
```

#### **🎯 Professional Confirmation Script:**
```
"Perfect! I have you scheduled for [DETAILS]. You'll receive a calendar 
invite at [EMAIL] with all the details. We'll also send a reminder 
[24 hours/day of] before your appointment. Is there anything else I can help you with?"
```

---

### **5. 🚫 Availability & Conflict Management**

#### **✅ Configure Availability Rules:**
```
"Booking constraints:
- Business hours: [YOUR_HOURS]
- Blackout dates: [HOLIDAYS, VACATION]
- Buffer time: [15 minutes between appointments]
- Same-day booking: [Allowed/Not allowed]
- Advance booking limit: [How far in advance]"
```

#### **🔧 Conflict Resolution Prompts:**
```
"When requested time isn't available:
'I don't have [REQUESTED_TIME] available. I have these options:
- [ALTERNATIVE_TIME_1]
- [ALTERNATIVE_TIME_2]  
- [ALTERNATIVE_TIME_3]
Which works better for you?'"
```

---

### **6. 💼 Business-Specific Optimizations**

#### **Medical/Dental Practices:**
```
"Additional prompts:
- 'Is this your first visit with us?'
- 'Do you have insurance we should know about?'
- 'Any medications or conditions to note?'
- 'Transportation or parking needs?'"
```

#### **Service Businesses (Plumbing, HVAC, etc.):**
```
"Service-specific questions:
- 'Can you describe the issue you're experiencing?'
- 'Is this an emergency or routine service?'
- 'Will someone be home during [TIME_RANGE]?'
- 'Any access issues we should know about?'"
```

#### **Restaurants:**
```
"Reservation specifics:
- 'How many people in your party?'
- 'Any dietary restrictions or allergies?'
- 'Special occasion we're celebrating?'
- 'Seating preferences (booth, patio, etc.)?'"
```

#### **Fitness/Wellness:**
```
"Class/session details:
- 'What's your experience level?'
- 'Any injuries or limitations?'
- 'First time with this instructor/class?'
- 'Do you have equipment or need to rent?'"
```

---

### **7. 🎭 Tone & Personality Configuration**

#### **✅ Professional Yet Friendly:**
```
"Personality guidelines:
- Be warm and welcoming, but efficient
- Use 'please' and 'thank you' appropriately
- Match the customer's energy level
- Stay professional even if customer is casual
- Always end with 'Is there anything else I can help you with?'"
```

#### **🏢 Brand Voice Examples:**

**Luxury Business:**
```
"Tone: Sophisticated, attentive, exclusive
'It would be my pleasure to arrange your appointment...'
'We look forward to providing you with exceptional service...'"
```

**Family-Friendly Business:**
```
"Tone: Warm, accommodating, understanding
'Absolutely! We love working with families...'
'No problem at all, we'll make sure everything works perfectly...'"
```

**Tech/Modern Business:**
```
"Tone: Efficient, knowledgeable, streamlined
'I can get that scheduled for you right away...'
'You'll receive all the details via email and text...'"
```

---

### **8. ⚠️ Error Handling & Edge Cases**

#### **✅ Prepare for These Scenarios:**
```
"Common edge cases to handle:
- Customer wants to book outside business hours
- Requested service not offered
- Same-day emergency bookings
- Cancellations and reschedules
- Multiple people booking for same time
- Unclear or incomplete information"
```

#### **🔧 Error Response Templates:**
```
"For unavailable times:
'Unfortunately, I don't have [REQUESTED_TIME] available. Would [ALTERNATIVE] work instead?'

For services not offered:
'We don't currently offer [SERVICE], but we do provide [SIMILAR_SERVICE]. Would you like to know more about that?'

For unclear requests:
'Just to make sure I get this right, are you looking for [CLARIFICATION]?'"
```

---

### **9. 📲 Integration & Follow-up**

#### **✅ Post-Booking Actions:**
```
"After successful booking:
1. Confirm calendar invite sent
2. Explain reminder system
3. Provide cancellation policy
4. Give contact info for questions
5. Thank them for choosing your business"
```

#### **🔄 Follow-up Script:**
```
"Great! Your appointment is confirmed for [DETAILS]. You should receive 
a calendar invite within a few minutes. We'll send you a reminder 
[TIMING] before your appointment. 

If you need to reschedule or cancel, just call us at [PHONE] or 
reply to the calendar invite. Thank you for choosing [BUSINESS_NAME]!"
```

---

## **🎯 Quick Setup Checklist for Business Owners**

### **⚡ 5-Minute AI Configuration:**
- [ ] Set current date/time and timezone
- [ ] Define business hours and blackout dates  
- [ ] Create default appointment title format
- [ ] Set standard appointment durations
- [ ] Configure required customer information
- [ ] Write confirmation script template
- [ ] Set brand voice and tone
- [ ] Add common service types and pricing
- [ ] Create alternative time offering script
- [ ] Set up post-booking follow-up message

### **🔧 Advanced Configuration (15+ minutes):**
- [ ] Service-specific questioning flows
- [ ] Emergency vs. routine booking procedures
- [ ] Multi-location handling
- [ ] Staff availability integration
- [ ] Pricing and payment discussion guidelines
- [ ] Cancellation and reschedule policies
- [ ] Special needs accommodation procedures
- [ ] Upselling and cross-selling opportunities

---

## **📊 Measuring AI Agent Success**

### **📈 Key Metrics to Track:**
- **Booking completion rate**: % of conversations that result in bookings
- **Information gathering accuracy**: % of bookings with complete details
- **Customer satisfaction**: Feedback on booking experience
- **No-show rates**: Impact of confirmation process
- **Average call duration**: Efficiency of booking process

### **🎯 Optimization Goals:**
- **>80% booking completion rate** for interested customers
- **<3 minutes average booking time** for standard appointments  
- **100% complete information** collection rate
- **<10% no-show rate** due to clear confirmations

---

## 🎯 **What This Actor Does**

- ✅ **Creates calendar events** in your Google Calendar via voice commands
- ✅ **Stores your Google credentials securely** for repeated use
- ✅ **Works with Retell.ai** and other MCP-compatible voice agents
- ✅ **Multi-tenant ready** - each business has isolated credentials
- ✅ **Real-time booking** during phone calls with customers

---

## 🚀 **Complete Setup Guide**

### **📋 Prerequisites**
- Google account with calendar access
- Apify account (free tier available)
- Retell.ai account or MCP-compatible AI agent

---

## **STEP 1: Get Google Calendar API Credentials**

### **1.1 Create Google Cloud Project**

1. **Go to [Google Cloud Console](https://console.cloud.google.com/)**
2. **Click "Select a project"** → **"NEW PROJECT"**
3. **Enter project name** (e.g., "My Calendar Integration")
4. **Click "CREATE"**

### **1.2 Enable Google Calendar API**

1. **In your project**, go to **"APIs & Services"** → **"Library"**
2. **Search for "Google Calendar API"**
3. **Click on it** → **Click "ENABLE"**

### **1.3 Configure OAuth Consent Screen**

1. **Go to "APIs & Services"** → **"OAuth consent screen"**
2. **Choose "External"** → **Click "CREATE"**
3. **Fill required fields:**
   - **App name**: "My Calendar App"
   - **User support email**: Your email
   - **Developer contact**: Your email
4. **Click "SAVE AND CONTINUE"** through all steps

### **1.4 Create OAuth 2.0 Credentials**

1. **Go to "APIs & Services"** → **"Credentials"**
2. **Click "CREATE CREDENTIALS"** → **"OAuth 2.0 Client IDs"**
3. **Application type**: "Web application"
4. **Name**: "Calendar Integration"
5. **Authorized redirect URIs**: Add `https://developers.google.com/oauthplayground`
6. **Click "CREATE"**
7. **💾 SAVE THESE VALUES:**
   - **Client ID**: `123456789.googleusercontent.com`
   - **Client Secret**: `GOCSPX-abcdef123456`

### **1.5 Add Yourself as Test User**

1. **Go to "OAuth consent screen"**
2. **Scroll to "Test users"** section
3. **Click "ADD USERS"**
4. **Enter your email address**
5. **Click "SAVE"**

### **1.6 Get Access & Refresh Tokens**

1. **Visit [Google OAuth 2.0 Playground](https://developers.google.com/oauthplayground)**
2. **Click Settings ⚙️** (top right)
3. **Check ✅ "Use your own OAuth credentials"**
4. **Enter your credentials:**
   - **OAuth Client ID**: Your client ID from Step 1.4
   - **OAuth Client Secret**: Your client secret from Step 1.4
5. **Click "Close"**
6. **In left panel**, find **"Calendar API v3"**
7. **Expand it** and **check ✅** `https://www.googleapis.com/auth/calendar`
8. **Click "Authorize APIs"**
9. **Sign in** to your Google account
10. **Click "Allow"** to grant permissions
11. **Click "Exchange authorization code for tokens"**
12. **💾 SAVE THESE VALUES:**
    - **Access token**: `ya29.a0Ae4lvC123...`
    - **Refresh token**: `1//0GWYz9XrP123...`

### **✅ You Now Have All 4 Required Credentials:**

| Credential | Example Value | Where You Got It |
|------------|---------------|------------------|
| **🔑 Access Token** | `ya29.a0Ae4lvC123...` | OAuth Playground |
| **🔄 Refresh Token** | `1//0GWYz9XrP123...` | OAuth Playground |
| **🆔 Client ID** | `123456789.googleusercontent.com` | Google Cloud Console |
| **🔐 Client Secret** | `GOCSPX-abcdef123456` | Google Cloud Console |

---

## **STEP 2: Set Up Your Apify Actor**

### **2.1 Access the Actor**

1. **Go to the actor**: [Google Calendar Create Event](https://apify.com/sambehnke/google-calendar-create-event)
2. **Click "Try for free"** or **"Start"**

### **2.2 Configure Your Google Credentials (One-Time Setup)**

1. **Fill in the Google credential fields:**
   - **🔑 Google Access Token**: Paste your `ya29.` token
   - **🔄 Google Refresh Token**: Paste your `1//` token
   - **🆔 Google Client ID**: Paste your client ID
   - **🔐 Google Client Secret**: Paste your client secret

2. **Fill in test event data:**
   ```json
   {
     "summary": "Test Event - Setup Verification",
     "description": "Testing Google Calendar integration",
     "start": {
       "dateTime": "2025-08-18T14:00:00-07:00",
       "timeZone": "America/Los_Angeles"
     },
     "end": {
       "dateTime": "2025-08-18T15:00:00-07:00",
       "timeZone": "America/Los_Angeles"
     },
     "attendees": [
       {
         "email": "test@example.com",
         "displayName": "Test User"
       }
     ]
   }
   ```

3. **Click "Start"**

4. **Verify Success**: Check the logs for:
   ```
   ✅ Credentials saved for future use
   ✅ Event created successfully!
   ```

5. **Check your Google Calendar** - you should see the test event!

---

## **STEP 3: Integrate with Retell.ai (or MCP Client)**

### **Option A: Direct Retell.ai Integration**

1. **In Retell.ai dashboard**, add a new MCP tool
2. **Configure the endpoint:**
   - **URL**: `https://api.apify.com/v2/acts/YOUR_USERNAME/google-calendar-create-event/runs`
   - **Method**: POST
   - **Headers**: 
     ```json
     {
       "Authorization": "Bearer YOUR_APIFY_API_TOKEN",
       "Content-Type": "application/json"
     }
     ```

3. **Test payload** (Retell.ai will send this):
   ```json
   {
     "eventData": {
       "summary": "Customer Appointment",
       "start": {"dateTime": "2025-08-18T16:00:00-07:00"},
       "end": {"dateTime": "2025-08-18T17:00:00-07:00"}
     }
   }
   ```

### **Option B: Use Apify's Official MCP Server**

1. **Configure your MCP client** with this URL:
   ```
   https://mcp.apify.com?token=YOUR_APIFY_TOKEN&actors=YOUR_USERNAME/google-calendar-create-event
   ```

2. **Example with your credentials:**
   ```
   https://mcp.apify.com?token=apify_api_YOUR_TOKEN&actors=sambehnke/google-calendar-create-event
   ```

3. **In Claude Desktop** (claude_desktop_config.json):
   ```json
   {
     "mcpServers": {
       "apify": {
         "type": "sse",
         "url": "https://mcp.apify.com/sse?token=YOUR_APIFY_TOKEN&actors=sambehnke/google-calendar-create-event"
       }
     }
   }
   ```

---

## **STEP 4: Voice Agent Usage**

### **🎙️ Example Voice Interactions**

**Customer**: *"I'd like to schedule an appointment for tomorrow at 2 PM"*

**AI Agent Response**: *"I'll schedule that appointment for you right now..."*

**→ AI automatically sends:**
```json
{
  "eventData": {
    "summary": "Appointment - [Customer Name]",
    "description": "Phone: [customer phone]\nRequested: Tomorrow 2 PM",
    "start": {"dateTime": "2025-08-19T14:00:00-07:00"},
    "end": {"dateTime": "2025-08-19T15:00:00-07:00"},
    "attendees": [{"email": "[customer email]", "displayName": "[Customer Name]"}]
  }
}
```

**AI Agent**: *"Perfect! I've scheduled your appointment for tomorrow, August 19th at 2 PM. You'll receive a calendar invite shortly."*

---

## **📊 Input Parameters Reference**

### **Required Input:**
- **`eventData`** (object) - The calendar event details (minimal: start/end times)

### **Optional Customer Information Parameters:**
*These parameters can be used or ignored based on your AI agent configuration*

| Parameter | Type | Description | AI Prompt Example |
|-----------|------|-------------|-------------------|
| `customerName` | string | Customer's full name | "Always collect the customer's full name" |
| `customerPhone` | string | Customer's phone number | "Ask for phone number" or "Do not require phone number" |
| `customerEmail` | string | Customer's email address | "Get email for calendar invite" or "Skip email collection" |
| `serviceType` | string | Type of service/appointment | "Always ask what service they need" |
| `specialNotes` | string | Special requests or notes | "Ask if they have any special requests" |

### **🎯 Flexible Configuration Examples:**

#### **Full Information Collection:**
```
AI Prompt: "Always collect: customer name, phone, email, and service type. 
Send as separate parameters: customerName, customerPhone, customerEmail, serviceType."

AI Sends:
{
  "customerName": "John Doe",
  "customerPhone": "555-1234", 
  "customerEmail": "john@email.com",
  "serviceType": "Consultation",
  "eventData": {
    "start": {"dateTime": "2025-08-18T14:00:00-07:00"},
    "end": {"dateTime": "2025-08-18T15:00:00-07:00"}
  }
}
```

#### **Minimal Information Collection:**
```
AI Prompt: "Only collect name and service type. Do not require phone or email."

AI Sends:
{
  "customerName": "Jane Smith",
  "serviceType": "Haircut", 
  "eventData": {
    "start": {"dateTime": "2025-08-18T16:00:00-07:00"},
    "end": {"dateTime": "2025-08-18T17:00:00-07:00"}
  }
}
```

#### **Traditional Approach (No Separate Parameters):**
```
AI Prompt: "Put all customer info in the event description. Do not use separate customer parameters."

AI Sends:
{
  "eventData": {
    "summary": "Appointment - Mike Johnson",
    "description": "Customer: Mike Johnson\nPhone: 555-9999\nService: Oil Change",
    "start": {"dateTime": "2025-08-18T10:00:00-07:00"},
    "end": {"dateTime": "2025-08-18T11:00:00-07:00"}
  }
}
```

### **🔄 How the Actor Processes Customer Parameters:**

When customer parameters are provided, the actor automatically:
- **Generates event title**: `"{serviceType} - {customerName}"` 
- **Builds description**: Organizes customer info professionally
- **Adds attendee**: Includes customer email if provided
- **Maintains flexibility**: Works with or without these parameters

### **EventData Parameters:**

| Parameter | Type | Required | Description | Example |
|-----------|------|----------|-------------|---------|
| `summary` | string | ❌* | Event title | "Doctor Appointment" |
| `start.dateTime` | string | ✅ | Start time (ISO 8601) | "2025-08-18T14:00:00-07:00" |
| `start.timeZone` | string | ❌ | Start timezone | "America/Los_Angeles" |
| `end.dateTime` | string | ✅ | End time (ISO 8601) | "2025-08-18T15:00:00-07:00" |
| `end.timeZone` | string | ❌ | End timezone | "America/Los_Angeles" |
| `description` | string | ❌* | Event details | "Annual checkup with Dr. Smith" |
| `location` | string | ❌ | Event location | "123 Medical Center Dr" |
| `attendees` | array | ❌* | List of attendees | `[{"email": "user@example.com", "displayName": "John Doe"}]` |

*Auto-generated from customer parameters if not provided

### **Additional Optional Parameters:**
- **`calendarId`** (string) - Calendar to use (default: "primary")

---

## **🔧 Common Use Cases**

### **Simple Appointment Booking**
```json
{
  "eventData": {
    "summary": "Consultation with John Doe",
    "start": {"dateTime": "2025-08-18T10:00:00-08:00"},
    "end": {"dateTime": "2025-08-18T11:00:00-08:00"},
    "location": "Office or Phone Call"
  }
}
```

### **Detailed Appointment with Customer Info**
```json
{
  "customerName": "Jane Smith",
  "customerPhone": "555-0123", 
  "customerEmail": "jane.smith@email.com",
  "serviceType": "Dental Cleaning",
  "specialNotes": "First visit, nervous about procedures",
  "eventData": {
    "start": {"dateTime": "2025-08-20T09:00:00-08:00"},
    "end": {"dateTime": "2025-08-20T10:00:00-08:00"},
    "location": "123 Dental Way, Suite 100"
  }
}
```

---

## **🛡️ Security & Privacy Features**

### **🔐 Credential Security**
- **Encrypted Storage**: All credentials encrypted in Apify Key-Value Store
- **No Logging**: Credentials never appear in run logs
- **Account Isolation**: Each business has completely separate credential storage
- **Auto-Refresh**: Uses refresh tokens to maintain access without re-authentication

### **📊 Data Handling**
- **No Data Retention**: Only stores credentials and creates calendar events
- **Your API Limits**: Uses your own Google Calendar API quotas
- **Audit Trail**: All operations logged for transparency (without sensitive data)

---

## **🔄 Multi-Tenant Architecture**

### **For Multiple Businesses:**

Each business gets their own setup:

1. **Business A**: 
   - Own Apify account
   - Own actor instance 
   - Own Google credentials
   - Own Retell.ai endpoint: `https://api.apify.com/v2/acts/BUSINESS_A/actor/runs`

2. **Business B**:
   - Own Apify account
   - Own actor instance
   - Own Google credentials  
   - Own Retell.ai endpoint: `https://api.apify.com/v2/acts/BUSINESS_B/actor/runs`

**Result**: Perfect isolation - Business A's customers book in Business A's calendar, Business B's customers book in Business B's calendar.

---

## **⚡ Performance & Reliability**

- **Runtime**: Typically completes in 3-8 seconds
- **Compute Cost**: ~0.01 Compute Units per event creation
- **Rate Limits**: Subject to your Google Calendar API limits (1,000 requests per 100 seconds)
- **Error Handling**: Automatic retry logic and clear error messages
- **Token Refresh**: Automatically refreshes expired access tokens

---

## **🆘 Troubleshooting**

### **Common Issues & Solutions**

**❌ "No stored Google credentials found"**
- **Solution**: Run the actor manually once with all 4 credential fields filled

**❌ "Request had invalid authentication credentials" (401 error)**
- **Solution**: Get fresh access token from OAuth Playground and re-run setup

**❌ "The app is currently being tested" (403 error)**
- **Solution**: Add your email as a test user in Google Cloud Console OAuth consent screen

**❌ "Invalid datetime format" (400 error)**
- **Solution**: Use ISO 8601 format: "2025-08-18T14:00:00-07:00"

**❌ "Calendar not found" (404 error)**
- **Solution**: Use "primary" for main calendar, or verify calendar ID exists

### **Getting Help**
- **Google Calendar API**: [Official Documentation](https://developers.google.com/calendar/api)
- **OAuth Setup**: [OAuth 2.0 Playground](https://developers.google.com/oauthplayground)
- **Apify Support**: [Apify Documentation](https://docs.apify.com/)

---

## **📱 Example Voice Agent Scenarios**

### **Restaurant Reservations**
*"Book a table for 4 people tomorrow at 7 PM"*
→ Creates calendar event with party size and time

### **Medical Appointments**  
*"Schedule my annual checkup for next Friday morning"*
→ Creates appointment with doctor and patient details

### **Service Bookings**
*"I need a plumber for Tuesday afternoon around 2 PM"*
→ Creates service call appointment with customer info

### **Consultation Calls**
*"Set up a consultation call for Monday at 10 AM"*
→ Creates calendar event with video call details

---

## **🏷️ Tags**

`google-calendar` `voice-agent` `retell-ai` `mcp` `appointment-booking` `ai-automation` `calendar-integration` `oauth` `apify-actor` `multi-tenant`

---

**🎉 Ready to automate your calendar bookings with voice commands? Follow this guide step-by-step and you'll have a fully functional AI booking system in under 30 minutes!**

---

*Built with ❤️ for seamless voice-powered calendar management*
