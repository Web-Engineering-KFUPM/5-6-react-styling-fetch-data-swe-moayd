# 5-6-react-styling-fetch-data — Feedback

## Submission

- **Lab:** 5-6-react-styling-fetch-data
- **Deadline (Riyadh / UTC+03:00):** 2026-03-04T20:59:00+03:00
- **Last commit time (from git log):** 2026-03-04T06:39:42Z
- **Submission marks:** **20/20** (On time)


## Files Checked

- Repo root (cwd): /Users/moaydshahat/5-6-react-styling-fetch-data-swe-moayd/5-6-react-styling-fetch-data
- Detected project root: /Users/moaydshahat/5-6-react-styling-fetch-data-swe-moayd/5-6-react-styling-fetch-data
- App: ✅ /Users/moaydshahat/5-6-react-styling-fetch-data-swe-moayd/5-6-react-styling-fetch-data/src/App.jsx
- SearchBar: ✅ /Users/moaydshahat/5-6-react-styling-fetch-data-swe-moayd/5-6-react-styling-fetch-data/src/components/SearchBar.jsx
- UserList: ✅ /Users/moaydshahat/5-6-react-styling-fetch-data-swe-moayd/5-6-react-styling-fetch-data/src/components/UserList.jsx
- UserCard: ✅ /Users/moaydshahat/5-6-react-styling-fetch-data-swe-moayd/5-6-react-styling-fetch-data/src/components/UserCard.jsx
- UserModal: ✅ /Users/moaydshahat/5-6-react-styling-fetch-data-swe-moayd/5-6-react-styling-fetch-data/src/components/UserModal.jsx

---

## TODO-by-TODO Feedback

### TODO 1: Bootstrap layout + spacing + UserList grid + empty state — **20/20**

**Checklist**
- ✅ App.jsx: <header> className EXACTLY "bg-primary text-white py-3 mb-4 shadow"
- ✅ App.jsx: <footer> className EXACTLY "bg-light py-4 mt-5"
- ✅ SearchBar.jsx: wrapper <div> className EXACTLY "mb-4"
- ✅ UserList.jsx: Empty state returns <Alert variant="info"> with exact message
- ✅ UserList.jsx: Grid uses <Row> and users.map(...)
- ✅ UserList.jsx: Each user renders <Col key={user.id} md={6} lg={4} className="mb-4">
- ✅ UserList.jsx: Inside each <Col>, renders <UserCard user={user} onUserClick={onUserClick} />

**Deductions / Notes**
- ✅ No deductions. Good job!

### TODO 2.1: Fetch users (App.jsx first useEffect) — **20/20**

**Checklist**
- ✅ Sets loading true at start (setLoading(true))
- ✅ Clears error at start (setError(null))
- ✅ Fetches from "https://jsonplaceholder.typicode.com/users"
- ✅ Converts response to JSON (res.json())
- ✅ Stores result into users + filteredUsers (setUsers(data) and setFilteredUsers(data))
- ✅ Checks response.ok and throws an Error when not ok (top-level)
- ✅ On error sets error message (setError(err.message) or setError(e.message))
- ✅ Always finally sets loading false (setLoading(false))

**Deductions / Notes**
- ✅ No deductions. Good job!

### TODO 2.2: Filter users by name (App.jsx second useEffect) — **20/20**

**Checklist**
- ✅ Second useEffect dependency array is exactly [searchTerm, users]
- ✅ If searchTerm is empty, sets filteredUsers to full users (setFilteredUsers(users))
- ✅ Filters from users (users.filter(...)) not filteredUsers
- ✅ Filter is by name only (user.name...) and case-insensitive includes()
- ✅ Sets filtered result (setFilteredUsers(filtered) or setFilteredUsers(<filter expr>))

**Deductions / Notes**
- ✅ No deductions. Good job!

### TODO 3: "View Details" button (UserCard.jsx) — **10/10**

**Checklist**
- ✅ Renders a Bootstrap <Button>
- ✅ Button text is exactly "View Details"
- ✅ onClick calls onUserClick and passes the current user object

**Deductions / Notes**
- ✅ No deductions. Good job!

### TODO 4: User details modal (UserModal.jsx) — **10/10**

**Checklist**
- ✅ Renders <Modal> with show={show} and onHide={onHide}
- ✅ Has title "User Details" inside <Modal.Title>
- ✅ Uses <Modal.Header closeButton>
- ✅ Body shows large avatar using className='user-avatar-large' and user.name.charAt(0)
- ✅ Body shows Name, Email, Phone, Website each in its own <p>
- ✅ Footer has ONE Close button that triggers onHide

**Deductions / Notes**
- ✅ No deductions. Good job!

---

## How marks were deducted (rules)

- JS/JSX comments are ignored (so starter TODO comments do NOT count).
- Checks are intentionally light: they look for key constructs and basic structure.
- Code can be in ANY order; repeated code is allowed.
- Common equivalents are accepted, and naming is flexible.
- Missing required items reduce marks proportionally within that TODO.
