print(" this file was created within RStudio")
print("And now it lives on GitHub")
# this is assigning variables 
 X <- 10
 Y <- 5
 
 # this to performing arithmetic operations
  sum <- X + Y
  difference <- X - Y
  Product <- X * Y
  quotient <- X / Y
  # these are  numeric, character, Logical, and integer type 
  num <- 3.14
  Char <- "hello world of R Programming"
  logical_val <- TRUE
  integer_val <- 42L
  # these also to create a numeric vector 
  vector <- c(1,2,3,4,5)
  # accessing elements in a vector
  second_element <- vector[2]
  # Modify elements
  vector[2] <- 10
  print("Updated vector:")
  print(vector)
# Creating a 3x3 matrix
matrix_data <- matrix(c(1:9), nrow = 3, ncol = 3)

# Accessing elements in a matrix
element <- matrix_data[2, 3]
print("Matrix:")
print(matrix_data)
print(paste("Element at position [2,3]:", element))
# Creating a data frame
df <- data.frame(
  Name = c("John", "Jane", "Alex"),
  Age = c(25, 30, 22),
  Gender = c("Male", "Female", "Male")
)

# Print the entire data frame
print("Data Frame:")
print(df)

# Access specific columns
print("Names in the data frame:")
print(df$Name)

# Adding a new column
df$Salary <- c(50000, 60000, 45000)
print("Updated Data Frame:")
print(df)
# Conditional if-else statement
age <- 20
if (age >= 18) {
  print("You are an adult.")
} else {
  print("You are a minor.")
}
# For loop example
for (i in 1:5) {
  print(paste("Current value of i:", i))
}

# While loop example
count <- 1
while (count <= 5) {
  print(paste("Count:", count))
  count <- count + 1
}
# Creating a simple function
add_numbers <- function(a, b) {
  return(a + b)
}

# Calling the function
result <- add_numbers(10, 20)
print(paste("Sum:", result))
# Reading a CSV file into a data frame
data <- read.csv("file.csv")

# Display the first few rows of the data
print(head(data))

# Writing a data frame to a CSV file
write.csv(df, "output.csv")
# Simple scatter plot
x <- c(1, 2, 3, 4, 5)
y <- c(2, 4, 6, 8, 10)

plot(x, y, main="Simple Scatter Plot", xlab="X-axis", ylab="Y-axis", col="blue")
