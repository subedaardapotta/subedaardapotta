from PIL import Image
import pytesseract

def scan_and_solve(image_path):
    try:
        # Open the image file
        image = Image.open(image_path)
        
        # Use Tesseract to extract text
        extracted_text = pytesseract.image_to_string(image)

        # Add your logic to solve the problem based on extracted_text
        # This might involve using external APIs or custom algorithms

        return extracted_text  # Replace this with the actual result
    except Exception as e:
        return f"Error: {e}"

# Example usage
image_path = "path/to/your/image.png"
result = scan_and_solve(image_path)
print(result)

