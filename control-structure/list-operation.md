# লিস্ট অপারেশন

এই চ্যাপ্টারে আমরা আলোচনা করবো list এর কিছু ব্যাসিক অপারেশন নিয়ে। আগের চ্যাপ্টারে আমরা দেখেছি কিভাবে একটি লিস্টের নির্দিষ্ট ইনডেক্সে থাকা একটি এলিমেন্টকে অ্যাক্সেস করা যায়। তাহলে এবার দেখি, কিভাবে একটা নির্দিষ্ট ইনডেক্সে বা পজিশনে নতুন কোন এলিমেন্ট যুক্ত করা যায়,

```python
my_numbers = [1, 2, 3, 5]
my_numbers[3] = 4
print(my_numbers)
```

আউটপুট,

```python
[1, 2, 3, 4]
```

অর্থাৎ `my_numbers` লিস্টের `3` পজিশনে আগে ছিল `5` এবং সেই অবস্থানে আমরা নতুন ভ্যালু সেট করলাম `4`. `my_numbers[3] = 4` এভাবে। আর তাই `my_numbers` লিস্ট প্রিন্ট করার ফলে আউটপুট আসলো এই লিস্টের আপডেটেড ভ্যালু গুলো।

**লিস্টের যোগ ও গুন**  
মজার ব্যাপার হচ্ছে string এর মত করে লিস্ট নিয়েও যোগ বা গুনের কাজ করা যায়। যেমন - নিচের উদাহরণটা দেখে নেই,

```python
first_list = [1, 2, 3]
print(first_list + [4, 5, 6])
print(first_list * 3)
```

আউটপুট,

```python
[1, 2, 3, 4, 5, 6]
[1, 2, 3, 1, 2, 3, 1, 2, 3]
```

**লিস্টের মধ্যের এলিমেন্ট চেক**  
কোন লিস্টের মধ্যে নির্দিষ্ট কোন এলিমেন্ট আছে কিনা সেটা চেক করার জন্য `in` অপারেটর ব্যবহার করা হয়। যদি এলিমেন্টটি লিস্টের মধ্যে এক বা একাধিকবার থাকে তাহলে এটি `True` রিটার্ন করে অন্যথায় `False` রিটার্ন করে।

উদাহরণ,

```python
fruits = ["apple", "orange", "pineappe", "grape"]

print("orange" in fruits)
print("rice" in fruits)
print("apple" in fruits)
```

আউটপুট,

```python
True
False
True
```

একই ভাবে এর সাথে `not` অপারেটর ব্যবহার করে কোন এলিমেন্টের অনুপস্থিতিও চেক করা যাতে পারে। যেমন -

```python
fruits = ["apple", "orange", "pineappe", "grape"]

print("orange" not in fruits)
print(not "rice" in fruits)
```

আউটপুট,

```python
False
True
```

