# ActiveDirectory-GroupManagement

Watch me build this lab here! *(Add Loom link)*

Create and manage Active Directory groups for clean access control and organized user management.

---

## 🧰 Tools Used

- Windows Server 2022  
- Active Directory Users and Computers (ADUC)

---

## 🪜 Steps (End-to-End)

1. **Connect to the Domain Controller**
   - RDP into your Windows Server VM where AD DS is installed.

2. **Open ADUC**
   - Open **Server Manager**
   - Go to **Tools → Active Directory Users and Computers**

3. **Choose Where the Group Will Live**
   - Select the correct domain
   - Click the Organizational Unit (OU) you want to store the group in

4. **Create the Group**
   - Right-click the OU → **New → Group**
   - Name the group: `SchoolGroup`
   - Select **Group scope** (as needed)
   - Select **Group type** (Security or Distribution)
   - Click **OK**

5. **Verify the Group Exists**
   - Refresh the OU view
   - Confirm `SchoolGroup` appears in the group list

6. **Manage Membership**
   - Right-click `SchoolGroup` → **Properties**
   - Open the **Members** tab
   - Click **Add**
   - Add the users you want in the group
   - Click **Apply → OK**

7. **Confirm Membership**
   - Reopen group properties
   - Confirm the member list shows the correct users

8. **Apply Group-Based Access (Optional)**
   - Assign permissions to a folder/share/app using the group instead of individual users
   - Validate access using a user account in the group

---

## ✅ Outcome

A domain group was created and managed successfully to simplify user administration and enable group-based access control.
