# Daily Linux Muscle Memory Drills

This document defines short, repeatable command-line drills.
The goal is to build comfort and reflexes through daily repetition,
not memorization or speed.

Time commitment: 10–15 minutes per day.

---

## Daily Warm-Up (2–3 minutes)

```

pwd
ls
cd ~
ls -la
history | tail -10

```

---
## FIle and Directory Drill ( (3-4 minutes)
```

mkdir drill-test
cd drill-test
touch file1.txt file2.txt
ls
cp file1.txt copy1.txt
mv file2.txt renamed.txt
ls -l
rm copy1.txt
cd ..
rm -r drill-test

```

---

## Viewing and Searching Drill (3-4 minutes)
```

touch sample.txt
echo "alpha" >> sample.txt
echo "beta" >> sample.txt
echo "gamma" >> sample.txt

cat sample.txt
grep "beta" sample.txt
wc -l sample.txt
less sample.txt
rm sample.txt

```

---

## System Awareness Drill (2-3 minutes)
```

whoami
id
uptime
free -h
df -h
ps aux | head

```

---

## Stretch Drill (Networking)
```

ip a
ss -tuln
ping -c 3 8.8.8.8

```

---
