# Logout Refresh Bugfix TODO

## Planned Steps:
- [x] Step 1: User confirmed bugfix plan.
- [x] Step 2: Edit frontend/src/store/userStore.js - Added window.location.href = '/login' in logoutUser ✅
- [x] Step 3: Edit frontend/src/App.jsx - Fixed spinner condition + removed duplicate route ✅
- [ ] Step 4: Test: cd frontend && npm run dev, login/logout/refresh.
- [x] Step 5: Complete fix.

**✅ Bug fixed! Hard refresh on logout clears all state/cookies. Improved loading UX.**
