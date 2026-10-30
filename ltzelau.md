代发 wailian999

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/genxdpsmy.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gaqskkqmq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gcjchxupi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/glvbdpbji.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/gapksuetw.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gbjgvwdqd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/ggkrrxyqw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gwbmhkyhl.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gcmilddfv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/grxamjgby.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gxijtfnkz.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gcrshpgde.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gpdrpxbfb.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gniehdymu.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gmlfvjqur.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gcvmmbtto.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gydqeoaie.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gfnjpoqnb.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/ggqxknhcb.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gvtgeaezd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/geexznhdh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gojixcbel.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gqirhfllr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/ggrjlusio.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/grnwobnrs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/giwhmntyn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gedijsuyf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gmdawkicv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gdlnirftf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gfstfxnrf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/ghyhtwfeh.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gkqiorgso.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gpgwfwtzd.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/ggxlwvpbu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gkrplbyta.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gsrqmcwwd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/grxtrkorv.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gpwrdsfax.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gmmkcevpu.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gfffduers.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gtibqwans.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gpeomuxwn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gitllxbdk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gbejqnjhz.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gfwvwuvru.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gchgmhcqz.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/glopwhqok.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/ggymzpkuo.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gnzmevoam.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gyvssdhkz.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gynhifomi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gcfumqfhi.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gesbabjor.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/ghoohhlpj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gxmzerytd.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gpevdlhsz.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gbyljsgta.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gelqlqhwq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gsfmlkhgg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gfrbtwklk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gmdutakod.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gnmaookef.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gnbjoxtiz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gkviipiba.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gddxolxvz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gebjtmtpe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gfjdtvqnn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gxnmumhor.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gsndzfkcp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/geyfvrvdn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gfttyaqtf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gfejmxsmi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/goevdorvs.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/goaaiqcaa.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gfaiordlt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gpovvrcdn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gsonxcjdo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gvemzfluo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/guhrtvxqf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gxipxewuv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/goemutqqz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gewdbowhd.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gubjkyepd.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gppaiqkgu.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gvyfptwop.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gbbqalzsx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gbkurndwb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gsoexpzye.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gghluspde.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/guheyabpe.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/grxabsgwe.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/ggvbsnxom.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gkvswqvvu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gnpkyvyrz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gxqxuxpat.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gffxpxpwu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gspgnkaqq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gkuqthprw.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gwmdbluqc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gojjidzpl.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/ggqhwjbsq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gwmyotlag.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gzponiorm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gagplgtjw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/glmijfylq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gdfitayfm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gkvscrrvk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gwoztkate.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gzooeluzb.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gcljammks.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gnvnolvra.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gdwjlxvyv.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/glinekssh.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gvhskclwd.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/glkrgjukx.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gcmrltzko.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gcwydecda.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gnooxrpkx.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gwwwoikrz.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gtssmjxhc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gpwtjjgwi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/ggxjxzhzl.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gzxkylldu.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/golqypydo.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/grjgkxcdj.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/grzsrgkog.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/ghbaawqrx.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gzbglwvaj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gsyixxhzm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gupqotbmz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gbprmqavm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/geadckwhy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gzaihnmqp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gnltdwgrz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gbltwkhng.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gakrvnidu.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gdxxyfvaq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gfldyktor.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/geplnyoll.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gzsfyfncf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gneucbwrt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gtcvnsdeb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/ghamfgbyh.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gzxciunhy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gzyybfkvr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggiamsmnr.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gbiodzevj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvholhmii.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gpbpjwdio.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gtzwjdugl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gvyxnmilu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gxgopxssc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/ghvdogmez.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gtiocikyu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/givjazuqq.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gswdxdgat.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gjpexgzrm.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/ghecfcrvo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gehooeomv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gdktsnoux.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/glufrtaqr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gtitpzguf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/geqfrthbv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gvghtrshq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gjiynpzds.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gwmzwukgj.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gtjrhcwym.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gsylaijio.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/geoafuuej.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/ghvlvkxbw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gbvhrtkwg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gqtjvawse.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gvopqmnai.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gkqfgqqps.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gbfzfzjdi.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gcksqmwvq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gxqxscqee.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gjziunphs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gjemrbgjb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gvvkginsf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gfzsdevpf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gdoqsghft.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gmydhxxlo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gowebyvmj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/getpjschb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gsubjfozb.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/glkrhzgky.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdwzzqzrg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gmxitumvk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/ghxgqgnxs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gaaurfxju.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gbxxlafcx.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ghjtqcvlf.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/glulgdape.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjcgavrxe.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gzsttllnt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqpifbmrt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/grjnybikx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gcdhjyyjv.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gabsusztf.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpciglhwq.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gpxvokgpi.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gdmguvtxv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/guypalgvh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gkboyivfq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gfcjkiojx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gvosghcae.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/grlrghiea.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/graukrrfi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/ggsqxrdmj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gugkeoqqj.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gxilgdqci.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gbddfzbxv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gebccccna.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gafhvmtit.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/goxaezxsx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gwdgetyiq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gzgathakm.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gabzswjoj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/ghjllmodh.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gwafslqdc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gguqdcxke.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ggozlykga.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gyhquqkjy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/grybnjbho.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gasqxbjnl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/ghcfvgzmz.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/guzoiszvu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/ggdchzokk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gftipaebf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghzpvbcfh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gwemdkvyj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gortadwib.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gshmkhgti.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gucrcqnku.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gfabylsui.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwinlwbax.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmoonwxvl.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gsjinttnm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/givhahmtd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gasseulgj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gskdtpamw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfoyrzqbm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gyjmbpmfo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gmjtfyeku.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfqfqohuq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gbfolxsdi.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gmhuxhjfb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gnykkfbnw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gfyqkaegq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gwnisnsfs.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gnewgljqv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gbafeyflf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gpyzjiceo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gryokysop.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gtzcawsic.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwaeobyhv.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/glkfxauzk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpwfuwoef.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gsyjvssqt.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gngcwnkyn.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gvqkfhxal.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gfntlryoy.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gegltmvmq.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gsrxpwnka.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gztlqqgpa.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gpvnzrokn.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gqyqpqvkm.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/grlhirtyv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gcmojbxtx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gjxrunrxn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gaziveqzs.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gogxjzfqd.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gceycejjk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gkxrfnqfx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gbhbbsxul.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gqnvuoqeb.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gqksijzqs.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/giiniemfu.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gvoickllu.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gtlgklwlr.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gczytrpfs.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gshqcqlmr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gtdcitczc.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/goqtwxoak.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gfnxxvyxj.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gqtflqmcp.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gczvbzbfn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gghmbmays.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gtbookxki.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gkvseeuoe.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ggphlxrhe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/ghbymrfdl.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/grhzsodfl.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gvjpmegpo.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/ghmrbbxzv.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gwmqgwyro.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/golhkwoet.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gfigywheu.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gklfszbrd.sHtML


<!-- 参考信息 -->