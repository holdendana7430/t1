代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nlerelmb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ltnlkgto.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nkvexsoe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3noyolune.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3pvihwkbb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sfhpyvnu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3hlmkhzdt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aiqyuvxu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uwctfjrq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gxjkhigc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rwtqbtio.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uiigzwxg.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3olsvynlb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fqhxkfmy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3kduvgrmj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hjrznjwm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3szkoinuk.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zylrdwoq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3vufsikbf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kpqyrodn.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3qagadmig.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3vmrnpvkm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3omgdiunn.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ldxxmwyh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3oyykrnjc.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qdowrqlx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kfbbtqgm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3prhuykzv.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3dkmvpces.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qjiisjvu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ootxqvif.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3tgistdlc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3vkdoueec.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3dfshlrmz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3fgwrscqe.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3drmgvahf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3bhwwkmdd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3twtapsty.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ffmrvlxu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3khnolbml.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3viacpqwo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ktqgjvmc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3qjlomdlh.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uarkaqzu.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zxzqeqps.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3insazozy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gyqqfeii.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gaelasuw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3irdhvabl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fphhmazf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3nhgspkfp.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3xgsjdvrm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kgikwivj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wmcmklby.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ututwfvi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3msadplsh.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uevbfvsf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3pkbqjffp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ivnbkcip.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3iolrjigi.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ekulaswr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bajiigiy.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3izcmlkjh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3jixmbmvs.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3lnwzgpys.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fnyeuwyd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3syivspjd.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qmgkmyhr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ohamzhet.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3yonyoeoz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfzbskay.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gqffluyf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lvyaggte.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mzbodday.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ycxjsife.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3aiisezxe.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3xgxnzeaz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3tisscmfy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3aijalnan.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3mjbyrems.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3elkocykn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ihvsvvgv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3qoifbqrc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3fwnisurw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fgpffyyj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3rjqnhznw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3hljvpooi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3wvhunezi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3opqrypal.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3owmgzlpb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3dvduunfh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3risczxlc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iqhufxld.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ijxpiuoq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3sngbgeab.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dweoclar.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3gvfooorb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lsabfefo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bauscfng.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ylzfnlhf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3zvrzhffh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3nuoirwot.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3uqpxlftu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3eygjsbzj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3nwuecast.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3jhmghwyp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rvvycdac.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3reoerfvy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3udvpsrge.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vhzuqyau.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vvmopeai.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3balafraa.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3eidopszk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3dowuyoku.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3gzqciakj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3elegzgrc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rwnqthtr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ukpouaks.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ayqpyuau.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jwutazev.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3yzwkkdrs.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3euelhugs.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3qjfmacgj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gbsamavt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3yqxpxgqa.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rihjsjqp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3osyqwala.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3gjnjgzev.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3skgxbfhh.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3tgpjuerw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3uyhxryez.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3dalgvujz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3iifckmtf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3clnqgnbu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3gvrxbenn.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zpwnozeu.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3kbszorjy.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3kxlacdcy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ubhhokcg.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3bxvlhjni.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3vlljihyo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vhjqbuqx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pipkvhsm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hcelmymm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3adiejxvb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3brfefopv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yizgqvwe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3actsxgrl.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3xlimbfdv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uweykmfr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mnnocgid.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nnmyymcc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vwetulrn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qzduvbqq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3fpocyann.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ctbllwev.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vlosdxny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lbpthjrt.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3mflfbdam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ecofzsjz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3zfmqgqxv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3seiyaofr.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ivamkzni.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3mzfiuarx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nwdzxonw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3faznweqe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3dvkgtemr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dolhqnkn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3miwnibrq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3vavjljtt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3bkrgxlgo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3shyhktdj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmkolykx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzpsgpbe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ytpvwmbt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3suremddu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3jqffvjgv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3grkofbat.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3mfrbknec.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zbyjvqxl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3wexnfooz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3npyhgjjk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nvafnpby.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ucbifdhs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3tmddvlhq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3mejhpbqe.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3efjrwdrd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3yaquqlyn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mncaejgx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3njlqlmmg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gtjvdcus.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3umncjwjk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3iadskzdi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jjyylvrk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3dxmrrtmb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3btkynqbg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ivrrmejh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3rogowxyl.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mxsrlkho.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3powmmzyb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ztwcycia.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3iqypeyla.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3oqoxnlws.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cbdwnayf.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3edwuxsbh.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3acwnhqzk.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jxpbxqyo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sdjsolhh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vbpbqubd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3paktsnkq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xwpqgzpc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lpgoqbal.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ufysfluy.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pheedanw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3iqputlti.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3juaguuit.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ccgulzzw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gjfhxnmh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3epfiuxee.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3opqyzzca.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3cilrjtkp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3xhomthsd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3mavobzwc.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3vkamoxhj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3hkhtozdy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjtxirzd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jsymwgzx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ovgihgmq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3emabzlxy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3rbzzzdav.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bvniyezy.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3bbkmmdtq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3kwbkshje.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iiyjnppk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vldqrmzy.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ttlriwqy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hhzetfth.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3siuctjlz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3dosddznc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gdssndnk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ukazppgn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3vsiyhgwd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hmcwegoc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3woncdvck.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ndlsylsi.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zntjzajf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3aldfnicw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rlcipihb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3exlhaopw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gvogglym.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3bxegtljt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3krtflomn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qybxuztm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3srgpwoco.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wwkznbtf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mobxhrip.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3bbgoitdk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pcsqxqmw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3myhdnnpq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3lxqoabjl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3sjfwtllo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3bzccjfwc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3etwqdrra.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3cgdjqehi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3sziztpbs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3pdzmjzfq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3tzmlivej.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3bejwogmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jqgdtoca.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3lklhnkrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jplpsbtb.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3dvvxlijg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3xabrgydd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3uaygzsvx.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qsadmaaq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3idrptlqn.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3jxhlsruq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3tohemryo.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ztfxrnbr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3olygspgt.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3eiisegjo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3xsbgtqty.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3alwjqpfc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bcatuacw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3srnhhydy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ghcronho.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3geucmggp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3eqyiwyku.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgroomyq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3kugqratc.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zboodiim.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rkecchte.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lpcewgzt.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ustseuwc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3aiqeopkv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3lqyoierv.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vjsugath.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3chxrljky.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3gjqvvcke.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vbpwlorn.html


<!-- 参考信息 -->