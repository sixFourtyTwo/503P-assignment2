# Fly Me Up — Conversational Agent

This system is a virtual assistant that acts as the charming aero-concierge for Fly Me Up, a whimsical company that transforms ordinary cars into enchanting, sky-surfing flying machines using its signature WingWhirl conversion ritual.

## What It Does

The system uses OpenAI’s function calling (tools) to process user requests and automatically call internal functions to:

- Save customer inquiries when potential flyers share their name, email, and message expressing interest in converting their car.
- Record unanswered questions whenever the assistant cannot respond confidently about flight conversions, levitation mechanics, or other aerial matters.
- Estimate flight conversion costs based on a customer’s vehicle value and conversion preference (“convert” or “trade”).
- All assistant interactions, including tool calls and responses, are logged for clarity, quality assurance, and magical accountability.

## Tools Implemented
- Tool Name:	Purpose	Output Log
- save_customer_inquiry:	Stores aspiring flyers’ contact details and messages in logs/customer_inquiries.jsonl	
- record_unanswered_question:	Captures unhandled or out-of-scope questions in logs/unanswered_questions.jsonl	
- estimate_flight_conversion_cost:	Calculates the transformation quote based on the car’s value and user option (“convert” or “trade”)	

## Conversion Options
- Convert (Lift & Drift): Transform your current car into a flying marvel for 44% of its market value (plus a complimentary jar of moonlight).
- Trade (Trade for the Skies): Sell your car to Fly Me Up for 80% of its value — we’ll convert and add it to our elite airborne fleet.
- Add-Ons (Personal Cloud Customization): Optional magical enhancements like glowing wings or meteor-proof shields for an additional 12% of the conversion cost.

All conversions are performed by our certified aero-mages, flightsmiths, and wind whisperers, ensuring your new ride remains safe, landable, and effortlessly airborne.

## Output Files
All generated logs are automatically stored in the /logs directory:
- customer_inquiries.jsonl — user contact and interest messages
- unanswered_questions.jsonl — logged unanswered or magical edge-case questions
- conversion_quotes.jsonl — estimated cost breakdowns for flight conversions