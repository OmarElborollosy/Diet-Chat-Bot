

# Diet and Nutrition Chatbot

## Overview

The Diet and Nutrition Chatbot is a Scala-based tool designed to assist users in creating and managing personalized diet plans. By analyzing food data and user profiles, the chatbot calculates Basal Metabolic Rate (BMR) and generates customized diet recommendations.

## Features

1. **Food Data Analysis**:
   - Reads and parses food data from a specified file.
   - Provides essential nutritional information for various food items.

2. **User Profile Management**:
   - Supports user profiles, including details such as height, weight, activity level, gender, and age.
   - Personalizes diet plans based on individual characteristics.

3. **BMR Calculation**:
   - Calculates the Basal Metabolic Rate (BMR) using user profile data.
   - BMR represents the energy expenditure required for basic bodily functions at rest.

4. **Diet Plan Generation**:
   - Generates and prints personalized diet plans.
   - Considers BMR, activity level, and nutritional requirements.

## Installation

To run this project, ensure you have Scala installed on your system. If not, download it from Scala's official website.

## Usage

1. **Clone the Repository**:
   - Clone the project repository to your local machine:

     ```
     git clone https://github.com/yehiamahrous/diet-nutrition-chatbot.git
     cd diet-nutrition-chatbot
     ```

2. **Compile and Run**:
   - Compile the main Scala file:

     ```
     scalac Main.scala
     ```

   - Execute the chatbot:

     ```
     scala NutritionChatbot
     ```

## File Structure

- `Main.scala`: Contains the chatbot implementation.

## Code Explanation

### Data Structures

- `Food`: A case class representing a food item with its nutritional values.
- `UserProfile`: A case class representing the user's profile.

### Functions

- `AnalyzeFoodData(filePath: String)`: Reads and parses food data from the specified file.
- `parseFoodLine(line: String)`: Parses a line of food data.
- `calculateBMR(user: UserProfile)`: Calculates the Basal Metabolic Rate (BMR) based on the user's profile.
- `printPlan(plan: List[Food], mealType: String)`: Prints the diet plan for a specific meal type.

## Limitations

- **No Support for Special Diets**:
  - The chatbot does not currently create diet plans for vegans, vegetarians, or individuals with specific dietary restrictions or allergies.
- **Limited User Profile Data**:
  - User profiles include basic attributes (height, weight, etc.), but other factors (medical conditions, fitness goals) are not considered.
- **Static Food Data**:
  - The chatbot relies on a static food data file and does not support dynamic updates or external food database integration.

## Future Enhancements

- **Special Diets**:
  - Add support for creating diet plans tailored to specific dietary needs (vegan, vegetarian, etc.).
- **Enhanced User Profiles**:
  - Incorporate additional user attributes (medical conditions, fitness goals) for more personalized recommendations.
- **Dynamic Food Data**:
  - Integrate with external food databases to provide up-to-date nutritional information.

## Example

1. Run the Scala code.
2. Create a user profile.
3. Ask the chatbot for a diet plan.
4. Provide necessary information to calculate BMR.
5. Receive a customized diet plan.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests for improvements or bug fixes.

