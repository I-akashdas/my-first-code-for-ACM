# my-first-code-for-ACM
This is my first GIT repository.
<br>
Author- Akash Das


// Define tax rates for different item types
const taxRates = {
    type1: 0.10,  // 10% tax on type1 items
    type2: 0.15,  // 15% tax on type2 items
    type3: 0.05,  // 5% tax on type3 items
    type4: 0.08   // 8% tax on type4 items
};

// Function to calculate tax and final amount
function calculateTax(itemType, amount) {
    const taxRate = taxRates[itemType.toLowerCase()] || 0; // Default to 0 if itemType not found
    const taxAmount = amount * taxRate;
    const finalAmount = amount + taxAmount;
    return { taxAmount, finalAmount };
}

// Example usage
const itemType = "type1"; // Change as needed
const amount = 80; // Change as needed

const result = calculateTax(itemType, amount);
console.log(`For ${itemType}, the tax amount is ${result.taxAmount} and the final amount is ${result.finalAmount}.`);




Output:=
For type1, the tax amount is 8 and the final amount is 88.



