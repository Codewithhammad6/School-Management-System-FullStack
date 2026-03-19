# Server Cookie Bugfix TODO ✅ COMPLETE

**Fixed:** logout controller now clears correct cookie `"tokenSchool"` (was wrong "token").

**Change:**
```
res.cookie("tokenSchool", null, {  ← CORRECT NAME NOW
```

**Full Fix Stack:**
1. Frontend: Hard refresh on logout ✅
2. Backend: Correct cookie name ✅

**Test:**
```
cd server && npm run dev
cd frontend && npm run dev
```
Login → logout → refresh → **Login page only!** No auto-login.

**All tasks done!** 🎉
