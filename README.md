# Multi-Instance Website User Tester

A powerful tool for simultaneous testing of web applications across multiple simulated user instances. This tool allows automated interaction testing, form filling, and user behavior simulation in parallel instances.

## 🚀 Features

### Core Capabilities
- Multiple simultaneous testing instances
- Real-time website interaction through iframes
- Automated user behavior simulation
- Live action logging with timestamps
- Dynamic instance management

### Interaction Types
- Random button clicking
- Automated form filling
- Scroll simulation
- Concurrent multi-instance testing

## 📋 Prerequisites

- Modern web browser (Chrome, Firefox, Safari, Edge)
- Websites must:
  - Be served over HTTPS
  - Allow iframe embedding
  - Have appropriate CORS policies

## 🛠️ Installation

1. Download both files:
   ```
   user-tester.html
   styles.css (optional - for custom styling)
   ```

2. Place files in your preferred directory

3. Open `user-tester.html` in a web browser

## 💻 Usage

### Basic Setup

1. Launch the tester:
   ```
   Open user-tester.html in your web browser
   ```

2. Enter target website URL:
   ```
   https://your-test-website.com
   ```

3. Add testing instances:
   ```
   Click "Add New Instance" button
   ```

### Testing Operations

#### Single Instance Testing
```javascript
1. Click "Click Random Button" to simulate button clicks
2. Click "Fill Random Form" to populate form fields
3. Click "Random Scroll" to simulate scrolling
```

#### Multi-Instance Testing
```javascript
1. Create multiple instances
2. Click "Interact With All" to simulate concurrent users
3. Monitor logs for each instance
```

### Log Monitoring
- Real-time logging of all actions
- Timestamp for each operation
- Scrollable log history
- Error reporting

## 🔧 Configuration Options

### Instance Configuration
```javascript
{
    id: number,          // Unique instance identifier
    sandbox: string,     // iframe sandbox permissions
    height: number,      // iframe height (pixels)
    width: number        // iframe width (pixels)
}
```

### Interaction Settings
```javascript
{
    scrollRange: number,   // Maximum scroll range
    inputPrefix: string,   // Prefix for generated form data
    clickDelay: number    // Delay between automated clicks
}
```

## ⚠️ Limitations

1. Security Restrictions
   - Cannot interact with sites blocking iframe embedding
   - Limited to HTTPS websites
   - Subject to CORS policies

2. Technical Limitations
   - No support for complex JavaScript interactions
   - Cannot handle file uploads
   - Limited to visible elements
   - No support for drag-and-drop operations

3. Browser Constraints
   - Some features may vary by browser
   - Performance depends on system resources
   - Memory usage increases with instance count

## 🔍 Troubleshooting

### Common Issues

1. Website Not Loading
   ```
   - Check if website allows iframe embedding
   - Verify HTTPS protocol
   - Check browser console for CORS errors
   ```

2. Interactions Not Working
   ```
   - Verify element visibility
   - Check for dynamic content loading
   - Inspect browser console for errors
   ```

3. Performance Issues
   ```
   - Reduce number of active instances
   - Clear browser cache
   - Check system resources
   ```

## 🛡️ Best Practices

1. Testing Strategy
   - Start with single instance testing
   - Gradually increase instance count
   - Monitor system performance
   - Log all critical interactions

2. Resource Management
   - Limit concurrent instances
   - Close unused instances
   - Clear logs periodically
   - Monitor memory usage

3. Security Considerations
   - Use test accounts only
   - Avoid testing on production
   - Monitor for unusual behavior
   - Review logs regularly

## 🔄 Future Improvements

- [ ] Support for authenticated sessions
- [ ] Custom interaction sequences
- [ ] Enhanced error handling
- [ ] Performance optimization
- [ ] Advanced logging features
- [ ] Custom event triggers
- [ ] Network condition simulation
- [ ] Test scenario recording

## 🤝 Contributing

1. Fork the repository
2. Create feature branch
3. Commit changes
4. Push to branch
5. Create Pull Request

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🙋‍♂️ Support

For issues, questions, or contributions:
1. Check existing issues
2. Create detailed bug reports
3. Include system specifications
4. Provide reproduction steps

## 🔗 Related Projects

- Selenium WebDriver
- Cypress
- Puppeteer
- TestCafe

## 📚 Additional Resources

- Web Security Documentation
- iframe Security Policies
- Browser Developer Tools
- Testing Best Practices

---

*Note: This tool is for testing purposes only. Please ensure you have permission to test on target websites and comply with all relevant terms of service and security policies.*