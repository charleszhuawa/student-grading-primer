# Edge Case
**1) Edge case identified:**  
When creating a new student, the `mark` field must between 0 and 100.  

- Invalid inputs include: negative numbers (e.g., -5), numbers greater than 100 (e.g., 101).  
- Without this check, invalid data could cause inconsistent database entries or errors in statistics calculations.

**2) How this is handled in the implementation:**  

In `app.py`, the following validation was added:

```python
if mark < 0 or mark > 100:
    return jsonify({"error": "Mark must between 0 and 100"}), 400