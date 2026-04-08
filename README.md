# Trello API Testing Project

A comprehensive API testing suite for the Trello platform, including detailed test cases, bug reports, and a complete Postman collection for API automation.

## 📋 Project Overview

This project contains comprehensive testing documentation and API automation tools for the **Trello API**. It includes:
- **API Test Cases** covering Board, List, Card, Checklist, Member, and CustomFields operations
- **Bug Reports** documenting issues found during testing
- **Postman Collection** with pre-configured requests for all API endpoints

## 📁 Project Structure

```
project-trello/
├── Project-trello_postman_collection.json  # Complete Postman API collection
├── project-_.xlsx                          # Test cases and bug reports
│   ├── board                               # Board API test cases
│   ├── bug of board                        # Board-related bugs
│   ├── list                                # List API test cases
│   ├── bug of list                         # List-related bugs
│   ├── card                                # Card API test cases
│   ├── bug of card                         # Card-related bugs
│   ├── checklist                           # Checklist API test cases
│   └── CustomFields-API                    # Custom Fields API test cases
└── README.md                               # This file
```

## 🔧 Features

### API Endpoints Covered

The Postman collection includes **7 main endpoint groups** with **100+ API requests**:

#### 1. **Board Operations**
- Create, Get, Update boards
- Add labels, lists, and descriptions
- Star boards and manage actions
- Get board information and statistics

#### 2. **List Operations**
- Create and manage lists
- Move lists between boards
- Archive/unarchive lists
- Get list cards and actions

#### 3. **Card Operations**
- Create and update cards
- Add attachments and stickers
- Manage comments and labels
- Add card members
- Create and manage checklists

#### 4. **Checklist Operations**
- Create and manage checklists
- Add and update checklist items
- Convert checklist items to cards

#### 5. **Member Management**
- Add members to boards
- Manage board memberships
- Member notifications and searches
- Custom emoji and sticker management
- Saved searches

#### 6. **Custom Fields**
- Create custom field definitions
- Add dropdown options
- Update and delete custom fields

#### 7. **Delete Operations**
- Delete boards, lists, cards, checklists
- Remove attachments and stickers
- Remove members and labels

## 🐛 Bug Reports

The project includes **3+ documented bugs**:

| Bug ID | Title | Severity | Priority |
|--------|-------|----------|----------|
| BUG_001 | List color not removed with null/empty value | Medium | Medium |
| BUG_002 | User can archive same list multiple times | Medium | High |
| BUG_003 | Additional bugs documented | - | - |

Each bug report includes:
- ✅ Bug description
- 📝 Steps to reproduce
- 🎯 Expected vs actual results
- 🖥️ Environment information
- 📎 Attachments and evidence links

## 🚀 Getting Started

### Prerequisites
- **Postman** (v9.0 or higher)
- **Trello API Key** and **API Token**
- Excel viewer for test cases

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/project-trello.git
   cd project-trello
   ```

2. **Import Postman Collection**
   - Open Postman
   - Click **Import** → **Upload Files**
   - Select `Project-trello_postman_collection.json`
   - Setup your environment variables

3. **Configure API Credentials**
   - Set `APIKey` collection variable
   - Set `APIToken` collection variable
   - Set `basic-url` to your Trello API endpoint

### Usage

#### Running API Tests in Postman

1. Open the imported collection
2. Set collection variables:
   - `APIKey`: Your Trello API key
   - `APIToken`: Your Trello API token
   - `basic-url`: `https://api.trello.com/1`

3. Run requests individually or use the Collection Runner for batch execution

#### Viewing Test Cases

1. Open `project-_.xlsx` in Excel
2. Navigate through different sheets:
   - `board` - Board API test cases
   - `list` - List API test cases
   - `card` - Card API test cases
   - `checklist` - Checklist API test cases
   - `bug of board`, `bug of list`, `bug of card` - Bug reports

## 📊 Test Coverage

| Module | Test Cases | Status |
|--------|-----------|--------|
| Board | 15+ | ✅ Complete |
| List | 13+ | ✅ Complete |
| Card | 20+ | ✅ Complete |
| Checklist | 8+ | ✅ Complete |
| Member | 23+ | ✅ Complete |
| Custom Fields | 5+ | ✅ Complete |
| Delete Operations | 20+ | ✅ Complete |

## 🔐 Environment Variables

Configure the following in Postman collection variables:

```json
{
  "APIKey": "your-api-key",
  "APIToken": "your-api-token",
  "basic-url": "https://api.trello.com/1",
  "boardId": "generated-board-id",
  "ListId": "generated-list-id",
  "cardId": "generated-card-id",
  "checkListId": "generated-checklist-id"
}
```

## 📝 Test Scenarios

### Board Testing
- ✅ Create new board
- ✅ Get board details
- ✅ Update board properties
- ✅ Add/manage board labels
- ✅ Remove board descriptions
- ✅ Star/unstar boards

### List Testing
- ✅ Create lists on boards
- ✅ Update list properties
- ✅ Archive/unarchive lists
- ✅ Move lists between boards
- ✅ Get list cards and actions

### Card Testing
- ✅ Create and update cards
- ✅ Add attachments
- ✅ Manage comments
- ✅ Add stickers
- ✅ Create checklists on cards

### Advanced Testing
- ✅ Custom field management
- ✅ Member management
- ✅ Notification handling
- ✅ Bulk operations

## 🐛 Known Issues

1. **List Color Removal** - Color field not clearing with null/empty values
2. **Archive Validation** - No error when archiving already-archived lists
3. Additional issues documented in the bug reports sheet

## 📞 API Documentation

- [Trello API Official Docs](https://developer.atlassian.com/cloud/trello/rest/api-group-boards/)
- [Postman API Reference](https://learning.postman.com/docs/)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -am 'Add improvement'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Create a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👤 Author

- **Project Lead**: QA Testing Team
- **Created**: 2024

## 📚 Additional Resources

- [Trello API Authentication](https://developer.atlassian.com/cloud/trello/guides/rest-api/authorization/)
- [Postman Documentation](https://learning.postman.com/)
- [API Testing Best Practices](https://www.postman.com/resources/postman-api-testing-guide/)

## 🎯 Next Steps

- [ ] Integrate with CI/CD pipeline
- [ ] Add automated test reports
- [ ] Setup Newman for command-line execution
- [ ] Add performance benchmarks
- [ ] Create detailed API documentation

---

**Last Updated**: April 2024  
**Status**: ✅ Active & Maintained

