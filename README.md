# persian-2-persian-corpus
A Parallel Corpus of Persian Sentences for Spell Checking


## Contents:

```
/persian-2-persian-corpus (208,655 sentence pairs)
    /train (516 images)
        src.txt (200,000 unedited sentences)
        tgt.txt (200,000 edited sentences)
    /dev (2,000 sentece pairs)
        src.txt (2,000 unedited sentences)
        tgt.txt (2,000 edited sentences)
    /test (6,655 sentence pairs)
        src.txt (6,655 unedited sentences)
		tgt.txt (6,655 edited sentences)
```


## details and exmaples:

This dataset consist of 200K pairs of unedited and edited Persian sentences. The unedited version of the sentences may have one or several of the following error types:
A.	Punctuation errors
```
	سرب سنگین‌ترین عنصر پایدار است
	سرب سنگین‌ترین عنصر پایدار است.
```
B.	Missing zero-width non-joiner (ZWNJ) character in compound words
```
	حفظ رقابتپذیری در اقتصاد بر اثر تضعیف پول ملی
	حفظ رقابت‌پذیری در اقتصاد بر اثر تضعیف پول ملی
```
C.	Missing space between consecutive words
```
	از دیگر مشخصات دصتگاه جدید ژاپنیها می توان به اباتری 3240 میلیآمپرساعتی و سیستم آمل اندروید پی اشاره کرد.
	از دیگر مشخصات دستگاه جدید ژاپنی‌ها می‌توان به باتری ۳۲۴۰ میلی‌آمپرساعتی و سیستم عامل اندروید پی اشاره کرد.
```
D.	Real-word errors (a misspelled word is a valid word in lexicon)
```
	در هفته گذشته نرخ عرض روند افزایشی داشت.
	در هفته گذشته نرخ ارز روند افزایشی داشت.
```
E.	Non-word spelling errors
```
	این تعادل موجب پایداری سطاره در این حالت می شود.
	این تعادل موجب پایداری ستاره در این حالت می شود.
```
F.	Using Arabic numerals (1, 2, 3, …., 9) in Persian texts
```
	بررسی رأی اعتماد وزیران پیشنهادی کابینهٔ دوم وی از روز یک شنبه 8 شهریور 1388 در مجلسآقاز شد .
	بررسی رأی اعتماد وزیران پیشنهادی کابینهٔ دوم وی، از روز یک‌شنبه ۸ شهریور ۱۳۸۸ در مجلس آغاز شد.
```
G.	Using English quotation mark in Persian texts (/“”/ instead of /«»/)
```
	او فرند " جهانبخش خوان پهلوان "  پسر " خسروخوان" بود.
	او فرزند «جهانبخش خان پهلوان»، پسر «خسرو خان» بود.
```