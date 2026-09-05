# Language layer: Indonesian

Load with `SKILL.md` **and** the matching register file, when the copy is in Indonesian. This file adds language-specific tells. It does not replace anything.

## Status of this file: not yet validated

The universal layer in `SKILL.md` is grounded in published work on machine-written text: corpus studies of excess vocabulary in 2024 publications, editorial guidance, and detection research. That work is almost entirely about English. Most register and layer files carry a provenance line of their own, and several state that they rest on field convention rather than on a corpus.

No equivalent corpus exists for Indonesian. The patterns below were derived inductively from a set of 18 synthetic Indonesian samples generated across the four registers that existed when this file was written (marketing, product UI, documentation, editorial), then grouped by shape. The seven registers added since have not been sampled in Indonesian at all. That method finds real patterns, but it can only find the ones present in the generator's own habits, and it cannot measure how often any of them occur in the wild.

Treat this file as a working hypothesis. It is separated from the register files precisely so it can be corrected or replaced wholesale without touching validated material. Patterns confirmed against real samples should be marked as such; patterns that never appear in real text should be deleted rather than left in.

## Why English rules do not transfer

- The em dash (CW-50) is rare in Indonesian typography. The equivalent connector habit is the spaced hyphen ` - `, and it carries the same tell.
- Indonesian has no articles, so filler takes different forms: intensifier stacking and formulaic connectives rather than "the fact that" constructions.
- Politeness particles (*ya*, *yuk*, *nih*, *deh*, *kok*) and honorific framing (*Bapak/Ibu*, *Anda*) have no English counterpart, and machine text overuses them in a distinctive way.
- English loanwords carry prestige in Indonesian marketing copy, so untranslated terms function as buzzwords in a way they cannot in English text.

## Tells, mapped to universal rules

### CW-28 Temporal and landscape openers

The most consistent Indonesian tell found. Almost every generated marketing sample opened this way.

- *Di era digital yang serba cepat ini*
- *Dalam dunia yang terus berkembang*
- *Di tengah persaingan bisnis yang semakin ketat*
- *Seiring perkembangan teknologi*

Delete without replacement. The paragraph is always intact without it.

### CW-29 Pivot sentence

- *Nah, di sinilah [produk] hadir*
- *[Produk] hadir sebagai solusi*
- *Di sinilah peran [produk] menjadi penting*

The verb *hadir* used of a product is the marker. Cut the hinge and state what the product does.

### CW-40 Signposting

- *Mari kita selami lebih dalam*
- *Yuk, kita bahas satu per satu*
- *Sebelum kita masuk ke pembahasan*
- *Artikel ini akan membahas secara mendalam*

### CW-41 Chatbot closers

Very strong in Indonesian, and often survives into published text because it reads as ordinary politeness.

- *Semoga bermanfaat*
- *Semoga artikel ini bermanfaat bagi Anda semua*
- *Jangan ragu untuk menghubungi kami*
- *Terima kasih atas kesabaran Anda*
- *Sampai jumpa di artikel berikutnya*
- *Demikian pembahasan kali ini*

In correspondence, *Semoga email ini menemui Bapak/Ibu dalam keadaan sehat* is the same pattern in formal dress.

### CW-10 Excess vocabulary

Two families. Native abstractions:

*solusi inovatif, merevolusi, secara signifikan, kunci utama, tepat guna, memberdayakan, mengoptimalkan, transformasi digital, komitmen, unggulan, terdepan, mumpuni*

And English loanwords used as prestige markers rather than for precision:

*seamless, powerful, clean, intuitive, passionate, solid, enterprise, insight, effortless*

The loanword family is the sharper tell, because a human writer usually reaches for a loanword when the Indonesian word is genuinely missing, and machine text reaches for it as decoration.

### CW-13 Intensifier stacking

*sangat* attached to nearly every adjective, often doubled with another intensifier: *sangat penting sekali*, *benar-benar sangat*, *amat sangat*. One intensifier does the work.

### CW-21 Negative parallelism

- *Tak hanya X, tetapi juga Y*
- *Bukan sekadar X, melainkan Y*
- *Bukan A, tapi B*
- Triple negation as a feature list: *Tanpa biaya tersembunyi, tanpa kontrak, tanpa ribet* (also CW-20)

### CW-20 Rule of three

Indonesian marketing copy defaults to triads even harder than English, and alliterative or rhyming triads are the strongest form: *mudah, cepat, dan aman* / *hemat, praktis, dan efisien*.

### CW-14 Formulaic connectives

*Penting untuk dicatat bahwa*, *Perlu diingat bahwa*, *Pada dasarnya*, *Oleh karena itu*, *Dengan demikian*, *Kesimpulannya* opening consecutive paragraphs. Individually ordinary, in sequence a tell.

### CW-57 Exclamation and urgency flood

- *Tunggu apa lagi?*
- *Daftar sekarang juga!*
- *Rasakan perbedaannya!*
- *Simpan postingan ini sebelum hilang dari beranda!*

### Particle warmth (maps to CW-60 and CW-42)

Politeness particles sprinkled to manufacture friendliness: *Silakan coba beberapa saat lagi ya!*, *Yuk, lengkapi profil Anda!*, *Tenang, kok*. One particle in a voice that uses particles is fine. A particle in every string is a machine performing warmth.

This cuts both ways. Indonesian copy stripped of every particle reads stiff and translated, which is CW-60. The register file decides: product UI takes very few, editorial takes the author's own habit.

### Pronoun repetition (maps to CW-26)

*Anda* opening or appearing in every sentence. Indonesian drops pronouns comfortably, so their relentless presence is machine cadence rather than natural rhythm.

### CW-04 Fabricated social proof, Indonesian shapes

Two recognisable forms:

- *Dipercaya oleh ribuan pengguna di seluruh Indonesia* with nothing named.
- Fabricated testimonials built from generic name plus generic company: *Budi Santoso, CEO PT Sukses Selalu*. The pattern is a common given name paired with a company named for an aspiration (*Maju*, *Jaya*, *Sukses*, *Sejahtera*). Treat any such pairing as a fabrication until the user confirms it is real.

### CW-11 Significance inflation

*menandai babak baru*, *bukti nyata komitmen*, *langkah strategis*, *salah satu pemain kunci di industri*, *membawa dampak positif bagi masyarakat luas*.

### CW-43 Generic positive conclusion

*Bersama, kita wujudkan masa depan yang lebih cerah*, *Perjalanan kami masih panjang dan kami sangat antusias*, *optimistis dapat terus memberikan dampak positif*.

### CW-27 Rhetorical question opener

*Pernahkah Anda merasa...?*, *Bingung memilih...?*, *Apakah Anda termasuk orang yang...?*

In FAQ, the same shape appears as a question answered with pure affirmation: *Apakah data saya aman? Tentu saja!* The exclamation replaces the answer.

### CW-50 Dash as connector

The em dash is uncommon, the spaced hyphen ` - ` used as an aside is its equivalent and carries the same tell. Replace with a comma, a period, or parentheses.

### CW-15 Generic CTAs, Indonesian defaults

*Mulai Sekarang*, *Coba Gratis*, *Pelajari Lebih Lanjut*, *Hubungi Kami*, *Selengkapnya*, *Klik di sini*. Apply the marketing register's test: name what happens on click.

## Thresholds

The universal thresholds in `SKILL.md` apply unchanged, with one adjustment: count words, not characters, and note that Indonesian affixation produces longer words, so a 200-word window covers noticeably more text than the English equivalent. Do not convert by character count.

## Gate additions

- [ ] No temporal opener and no *hadir* pivot (CW-28, CW-29)
- [ ] No *Semoga bermanfaat* class closer (CW-41)
- [ ] English loanwords present only where the Indonesian word is genuinely missing
- [ ] *sangat* and other intensifiers not stacked (CW-13)
- [ ] *Anda* not in every sentence
- [ ] Politeness particles match the register, neither flooded nor stripped
- [ ] Any testimonial with a generic name and an aspirational company name verified as real (CW-04)
