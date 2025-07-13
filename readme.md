# Super Duper Guide - Test Automation Project

A personal test automation project built with Katalon Studio for automated testing of web applications, specifically focusing on contact form functionality and UI testing.

## 🚀 Project Overview

This project contains automated test scripts for testing web application functionality including:
- Contact form submission testing
- UI element validation
- End-to-end testing scenarios

## 📋 Prerequisites

Before running this project, ensure you have the following installed:

- **Katalon Studio** (version 5.9.0 or higher)
- **Java Development Kit (JDK)** 8 or higher
- **Web browsers** (Chrome, Firefox, Safari, Edge) for cross-browser testing
- **Git** for version control

## 🛠️ Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/super-duper-guide.git
   cd super-duper-guide
   ```

2. **Open in Katalon Studio**
   - Launch Katalon Studio
   - Go to `File` → `Open Project`
   - Navigate to the cloned repository folder
   - Select the `super-duper-guide.prj` file

3. **Configure Project Settings**
   - Update browser settings in `Profiles/` if needed
   - Configure test execution settings in `settings/`

## 🏃‍♂️ Running Tests

### Running Individual Test Cases
1. Navigate to `Test Cases/` folder
2. Right-click on the desired test case (e.g., `Send message through contactUs`)
3. Select `Run` → Choose your preferred browser

### Running Test Suites
1. Navigate to `Test Suites/` folder
2. Right-click on `Test Suite.groovy` or `Test Suite.ts`
3. Select `Run` → Choose execution profile

### Command Line Execution
```bash
# Run specific test suite
katalon -runMode=console -projectPath="path/to/super-duper-guide" -retry=0 -testSuitePath="Test Suites/Test Suite"

# Run with specific browser
katalon -runMode=console -projectPath="path/to/super-duper-guide" -browserType="Chrome" -retry=0 -testSuitePath="Test Suites/Test Suite"
```

## 📁 Project Structure

```
super-duper-guide/
├── Test Cases/                    # Individual test cases
│   └── Send message through contactUs.tc
├── Test Suites/                   # Test suite collections
│   ├── Test Suite.groovy         # Groovy test suite
│   └── Test Suite.ts             # TypeScript test suite
├── Object Repository/             # UI element repositories
│   └── Page_Development, Design, Video and Data en_ee6ba8/
├── Profiles/                      # Execution profiles
├── Scripts/                       # Custom scripts and utilities
├── Reports/                       # Test execution reports
├── Include/                       # External libraries and dependencies
├── settings/                      # Project configuration
├── console.properties            # Console configuration
├── .gitignore                    # Git ignore rules
└── super-duper-guide.prj         # Main project file
```

## 🧪 Test Cases

### Current Test Cases
- **Send message through contactUs**: Tests the contact form functionality including form validation and submission

### Adding New Test Cases
1. Right-click on `Test Cases/` folder
2. Select `New` → `Test Case`
3. Define test steps using Katalon's built-in keywords
4. Add assertions and validations as needed

## 📊 Test Reports

Test execution reports are automatically generated in the `Reports/` folder:
- **HTML Reports**: Detailed test execution results
- **PDF Reports**: Summary reports for stakeholders
- **JUnit Reports**: For CI/CD integration

## 🔧 Configuration

### Browser Configuration
- Configure browser settings in `Profiles/default.glbl`
- Supported browsers: Chrome, Firefox, Safari, Edge, IE

### Test Data Management
- External test data can be stored in `Data Files/`
- Support for Excel, CSV, and database connections

## 🤝 Contributing

Since this is a personal project, contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-test`)
3. Add your test cases or improvements
4. Commit your changes (`git commit -m 'Add new test case for XYZ'`)
5. Push to the branch (`git push origin feature/new-test`)
6. Create a Pull Request

## 📝 Best Practices

- **Page Object Model**: Use Object Repository for maintainable test scripts
- **Data-Driven Testing**: Utilize external data files for test data
- **Reusable Components**: Create custom keywords for common actions
- **Proper Assertions**: Always include meaningful assertions in test cases
- **Test Documentation**: Document test cases with clear descriptions

## 🐛 Troubleshooting

### Common Issues
- **Browser Driver Issues**: Ensure WebDriver is compatible with browser version
- **Element Not Found**: Check if Object Repository locators are up-to-date
- **Test Execution Failures**: Review test logs in Reports folder

### Debug Mode
- Use Katalon's built-in debugger for step-by-step execution
- Add breakpoints in test scripts for detailed investigation

## 📞 Support

For questions or issues:
- Check the [Katalon Documentation](https://docs.katalon.com/)
- Review test execution logs in the `Reports/` folder
- Create an issue in this repository for project-specific problems

## 📄 License

This project is for personal use and learning purposes.

---

**Happy Testing!** 🎉
