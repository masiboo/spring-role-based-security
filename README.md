# spring-role-based-security

🔧 How It Works Behind the Scenes:
✅ @PreAuthorize uses Spring Expression Language (SpEL) to evaluate security rules before entering the method.

✅ hasRole('XYZ') internally looks for authorities named ROLE_XYZ.

✅ Spring Security adds the "ROLE_" prefix automatically to roles declared using roles("ADMIN").

Summary:  
✅ @Secured("ROLE_ADMIN") checks for a specific role at the method level.

✅ Good for simple role-based access.

✅ Use @PreAuthorize(...) when you need more advanced logic or expressions.


