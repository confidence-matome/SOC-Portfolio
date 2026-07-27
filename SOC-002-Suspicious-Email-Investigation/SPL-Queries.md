# SPL Queries

Although this investigation focused on email header analysis, the following Splunk searches could be used to locate similar emails inside an enterprise environment.

## Search by Sender

```spl
index=email sender="Mantra Falcon"
```

---

## Search by Subject

```spl
index=email subject="Sr. AI Engineer opening"
```

---

## Search by Recipient

```spl
index=email recipient="xmarksthespot@gmail.com"
```

---

## Search by Domain

```spl
index=email "*terrigenisis.com*"
```

---

## Search by Keywords

```spl
index=email ("AI Engineer" OR sponsorship OR visa)
```
