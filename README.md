# NeuroNexus
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Web Form</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      background-color: #f3f4f6;
      font-family: 'Helvetica Neue', sans-serif;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      padding: 40px 20px;
    }
    .form-wrapper {
      background-color: #ffffff;
      padding: 40px 35px;
      border-radius: 16px;
      width: 100%;
      max-width: 500px;
      box-shadow: 0 12px 32px rgba(0, 0, 0, 0.1);
    }
    .form-wrapper h1 {
      text-align: center;
      font-size: 24px;
      color: #1f2937;
      margin-bottom: 30px;
      font-weight: 600;
    }
    label {
      display: block;
      margin-top: 18px;
      margin-bottom: 6px;
      font-size: 14px;
      color: #374151;
    }
    input,
    select,
    textarea {
      width: 100%;
      padding: 12px 14px;
      font-size: 14px;
      border: 1px solid #d1d5db;
      border-radius: 10px;
      background-color: #f9fafb;
      transition: border-color 0.3s, box-shadow 0.3s;
    }
    input:focus,
    select:focus,
    textarea:focus {
      outline: none;
      border-color: #6366f1;
      box-shadow: 0 0 0 3px rgba(99, 102, 241, 0.2);
      background-color: #ffffff;
    }
    textarea {
      resize: vertical;
      min-height: 100px;
    }
    .gender-options {
      display: flex;
      gap: 15px;
      margin-top: 10px;
    }
    .gender-options label {
      font-weight: normal;
      color: #4b5563;
      font-size: 14px;
    }
    .submit-btn {
      width: 100%;
      padding: 14px;
      margin-top: 30px;
      background-color: #4f46e5;
      color: #ffffff;
      border: none;
      border-radius: 10px;
      font-size: 15px;
      font-weight: 600;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }
    .submit-btn:hover {
      background-color: #4338ca;
    }
  </style>
</head>
<body>
  <form class="form-wrapper">
    <h1>Web Form</h1>
    <label for="fullname">Full Name</label>
    <input type="text" id="fullname" name="fullname" required>
    <label for="phone">Contact Number</label>
    <input type="tel" id="phone" name="phone" required>
    <label for="address">Address</label>
    <textarea id="address" name="address" required></textarea>
    <label for="company">Company Name</label>
    <input type="text" id="company" name="company" required>
    <label for="email">Email Address</label>
    <input type="email" id="email" name="email" required>
    <label for="dept">Department</label>
    <select id="dept" name="dept" required>
      <option value="">Select</option>
      <option value="HR">HR</option>
      <option value="Sales">Sales</option>
      <option value="Development">Development</option>
      <option value="Marketing">Marketing</option>
      <option value="Others">Others</option>
    </select>
    <label>Gender</label>
    <div class="gender-options">
      <label><input type="radio" name="gender" value="Male" required> Male</label>
      <label><input type="radio" name="gender" value="Female"> Female</label>
      <label><input type="radio" name="gender" value="Prefer not to say"> Prefer not to say</label>
    </div>
    <button type="submit" class="submit-btn">Submit</button>
  </form>
</body>
</html>
