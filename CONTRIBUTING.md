# 🤝 Contributing to EaseShop

EaseShop projesine katkıda bulunduğunuz için teşekkürler! Bu rehber, katkı sürecini kolaylaştırmak için hazırlanmıştır.

## 🚀 Hızlı Başlangıç

### 1. Repository'yi Fork Edin
```bash
# GitHub'da "Fork" butonuna tıklayın
# Kendi hesabınıza fork'u clone edin
git clone https://github.com/YOUR_USERNAME/easeshop.git
cd easeshop
```

### 2. Development Environment Kurulumu
```bash
# Bağımlılıkları yükleyin
npm install

# Development server'ı başlatın
npm run dev
```

### 3. Branch Oluşturun
```bash
# Ana branch'den güncel kodu çekin
git checkout main
git pull upstream main

# Yeni feature branch oluşturun
git checkout -b feature/amazing-feature
```

## 📋 Contribution Types

### 🐛 Bug Fixes
- Bug report issue'su oluşturun
- Sorunu reproduce edin
- Fix'i implement edin
- Test edin ve PR gönderin

### ✨ New Features  
- Feature request issue'su oluşturun
- Design/mockup paylaşın
- Implementation plan yapın
- Code review sonrası merge

### 📚 Documentation
- README güncellemeleri
- Code comment'leri
- API documentation
- Tutorial'lar

### 🎨 UI/UX Improvements
- Design improvements
- Accessibility enhancements
- Mobile responsiveness
- Performance optimizations

## 🔧 Development Guidelines

### Code Style
- **TypeScript**: Strict mode enabled
- **ESLint**: Follow project configuration
- **Prettier**: Auto-formatting enabled
- **Naming**: camelCase for variables, PascalCase for components

### Component Guidelines
```typescript
// ✅ Good component structure
interface ComponentProps {
  id: string;
  title: string;
  onClick?: () => void;
}

export default function Component({ id, title, onClick }: ComponentProps) {
  const [state, setState] = useState();
  
  return (
    <div className="p-4">
      <h2>{title}</h2>
    </div>
  );
}
```

### State Management
```typescript
// ✅ Zustand store usage
const items = useCartStore((state) => state.items);
const addItem = useCartStore((state) => state.addItem);

// ❌ Avoid destructuring entire store
const { items, addItem, removeItem } = useCartStore();
```

### Styling
```tsx
// ✅ Tailwind CSS classes
<div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-4">

// ✅ Responsive design
<button className="w-full md:w-auto px-4 py-2">

// ❌ Avoid inline styles
<div style={{ padding: '16px' }}>
```

## 🧪 Testing

### Before Submitting
```bash
# Lint check
npm run lint

# Type check  
npm run type-check

# Build verification
npm run build

# Manual testing
npm run dev
```

### Test Scenarios
- [ ] Feature works as expected
- [ ] Responsive design (mobile/tablet/desktop)
- [ ] Cross-browser compatibility
- [ ] Accessibility (keyboard navigation, screen readers)
- [ ] Performance (no unnecessary re-renders)

## 📝 Commit Guidelines

### Commit Message Format
```
type(scope): description

feat(cart): add quantity update functionality
fix(auth): resolve login validation issue
docs(readme): update installation guide
style(navbar): improve mobile responsiveness
refactor(store): migrate to Zustand
test(products): add unit tests
chore(deps): update dependencies
```

### Types
- **feat**: New feature
- **fix**: Bug fix  
- **docs**: Documentation
- **style**: Code formatting/UI improvements
- **refactor**: Code restructuring
- **test**: Adding tests
- **chore**: Build/config changes

## 🔀 Pull Request Process

### 1. Create Pull Request
- Use PR template
- Provide detailed description
- Include screenshots for UI changes
- Reference related issues

### 2. Code Review
- Address all review comments
- Ensure CI/CD passes
- Get approval from maintainers
- Squash commits if needed

### 3. Merge
- Maintainers will merge after approval
- Delete feature branch after merge
- Update local repository

## 🏷️ Issue Guidelines

### Bug Reports
- Use bug report template
- Provide reproduction steps  
- Include environment details
- Attach screenshots/videos

### Feature Requests
- Use feature request template
- Explain the problem it solves
- Provide use cases
- Include mockups/designs

### Questions
- Check existing issues first
- Use GitHub Discussions
- Provide context and details
- Tag relevant maintainers

## 🎯 Project Priorities

### High Priority
- 🐛 **Bug fixes** - User-facing issues
- ⚡ **Performance** - Core Web Vitals improvements
- 📱 **Mobile experience** - Responsive design
- ♿ **Accessibility** - WCAG compliance

### Medium Priority  
- ✨ **New features** - Enhanced functionality
- 🎨 **UI improvements** - Better user experience
- 📚 **Documentation** - Developer resources
- 🧪 **Testing** - Automated testing

### Low Priority
- 🔧 **Refactoring** - Code quality improvements
- 📊 **Analytics** - Usage tracking
- 🌐 **i18n** - Internationalization
- 🔌 **Integrations** - Third-party services

## 🛡️ Security

### Reporting Security Issues
- **DO NOT** create public issues for security vulnerabilities
- Email security concerns to: [security-email]
- Include detailed reproduction steps
- We'll respond within 48 hours

### Security Guidelines
- Never commit API keys or secrets
- Sanitize user inputs
- Use HTTPS for all requests
- Follow OWASP guidelines

## 📚 Resources

### Documentation
- [README.md](README.md) - Project overview
- [TEAM_DEVELOPMENT.md](TEAM_DEVELOPMENT.md) - Team workflow
- [Next.js Docs](https://nextjs.org/docs) - Framework guide
- [Tailwind Docs](https://tailwindcss.com/docs) - Styling guide

### Tools
- [GitHub Issues](https://github.com/mertdrmz/easeshop/issues) - Bug reports
- [GitHub Discussions](https://github.com/mertdrmz/easeshop/discussions) - Questions
- [VSCode Extensions](.vscode/extensions.json) - Recommended tools

## 🙏 Recognition

### Contributors
All contributors will be recognized in:
- README.md contributors section
- GitHub contributors page
- Release notes (for significant contributions)

### Maintainers
Current maintainers:
- [@mertdrmz](https://github.com/mertdrmz) - Project Lead

## 📞 Getting Help

### Communication Channels
- **GitHub Issues** - Bug reports, feature requests
- **GitHub Discussions** - Questions, ideas, general discussion
- **Pull Requests** - Code review and feedback

### Response Times
- **Bug reports**: 24-48 hours
- **Feature requests**: 3-5 days  
- **Pull requests**: 2-3 days
- **Questions**: 24 hours

---

## 🚀 Thank You!

Her türlü katkı değerlidir:
- 🐛 Bug reports
- ✨ Feature suggestions  
- 📚 Documentation improvements
- 🔧 Code contributions
- ⭐ GitHub stars
- 📢 Project sharing

**Happy Contributing!** 🎉

---

*Bu doküman sürekli güncellenmektedir. Önerileriniz için issue açabilirsiniz.*