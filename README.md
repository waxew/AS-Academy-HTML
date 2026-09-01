# AS Academy HTML

اپلیکیشن/ورودی اختصاصی دوره جامع HTML در AS Academy.

## معماری

این ریپو یک **Thin Course App** است و محتوای آموزشی یا UI مشترک را fork نمی‌کند.

```text
AS-Academy-HTML
      |
      v
AS-Academy-MainUi
      |
      v
AS-Academy-Core
      ^
      |
AS-Academy-MainCourse/courses/html/course
```

- محتوای دوره: `AS-Academy-MainCourse/courses/html/course`
- رابط مشترک: `AS-Academy-MainUi`
- موتور، Navigation، Search، Progress، Quiz، Exercise و Offline data: `AS-Academy-Core`
- Web entry فعلی: `index.html`

## دوره HTML

دوره به چهار سطح `مبانی / مقدماتی / پیشرفته / تخصصی` تقسیم شده و شامل درس فارسی، مثال کد، تمرین، Quiz، پروژه مرحله‌ای، Capstone، Glossary و References است.

محورها شامل ساختار سند، text semantics، link و URL، image و responsive image، table، form، Semantic HTML، media، metadata و SEO، Accessibility، RTL/i18n، Web Platform، Performance، Security/Privacy، Structured Data و Production Audit هستند.

## قانون توسعه

تغییر محتوای آموزشی باید در MainCourse انجام شود. قابلیت UI قابل استفاده برای چند Course باید در MainUi و منطق مشترک در Core پیاده‌سازی شود. این ریپو فقط branding/config/entrypoint اختصاصی HTML را نگه می‌دارد.
