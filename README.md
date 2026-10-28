# Service Sheets

Turns the restaurant's booking CSV export into clean, printable A4 service sheets: one for the early service (afternoon tea) and one for dinner.

**Live:** https://niceworklad.github.io/ServiceSheets/

## Using it

1. Export the day's bookings as CSV.
2. Open the page and drop the CSV on it (or click the box to choose it).
3. Check the sheets, edit any cell if something needs changing, then print.

The CSV needs a header row with at least a `Time` column. The tool also reads `Name`, `Covers`, `Table(s)`, `Booking`, `Guest Comments` and `Special offers and promotions`.

## What it does

- Splits bookings into the Early and Dinner sheets using the service times in Settings
- Tags guest comments for **allergies**, severe allergies, dietary needs, occasions and access needs, using keyword lists you can edit
- Warns about over-capacity bookings and tables that aren't on the plan
- Shrinks text to fit each sheet on one A4 page
- Tick box per booking, editable cells, column order and visibility, portrait or landscape, black and white or colour

Allergy tags are a prompt, not a guarantee: they only catch what was typed into the booking. Always confirm allergies with the guest at the table.

## Privacy

Everything happens in the browser. The page makes no network requests and the CSV is never uploaded. Settings are stored in the browser's local storage on that computer only.

## Files

- `index.html`: the whole tool in one file, including the embedded font
- `samples/`: example CSVs with made-up bookings for trying it out
- `fonts/OFL-Atkinson-Hyperlegible.txt`: licence for the embedded Atkinson Hyperlegible font (Braille Institute, SIL Open Font License 1.1)
