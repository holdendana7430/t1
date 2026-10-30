代发 wailian999

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/goraqzqrn.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gkxgexnpa.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gpvjjzhog.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gsacxhckj.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gfssrbeft.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gqfeusyss.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/giqykasoi.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gwhstcsjl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/ggtyniduk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gmloxrfco.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/ghzcpqknn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gqswaqvft.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gznkdvynt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gohyzuetb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/ghbuwbeum.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/glwilytaq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/ghzulyuec.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gjqznofdm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/giwbdwtaw.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gdtflvcnm.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gmmabgliy.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gycrypjxj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/guuyqyjug.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gllercxkr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gqsonqzdw.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gixbtzdki.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gkzkrcvrn.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gnszjwvll.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gygrxeqnr.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/ggtkmmbuh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gnwpmcfuu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/genirqaty.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/groowrfst.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gcpxdysuq.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gvjhjxrlz.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gwbooevbo.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gtrrpbpyl.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gpmbrsicv.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/givwybstx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/ginnxrwso.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gwoatciac.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gqkpmtnyn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gomcgmxqp.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gbfrintjv.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/godcyjadx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/guokccazm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/glczshuwc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gsyjgxskk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gximkxosf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gjgqxikqv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/ghcqxjgxd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/ggnmnppur.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gqcebvibv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/gsswtpacn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gzhyxhxwr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gffiuboap.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gwbxebdwj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/ghcntpyxc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gtecrrdjt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/ggxurqaeo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gjcytzkcn.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gehdrmear.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gjjnxgcdl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gwmrkglrx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/geiduorno.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gsqpminjw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gtobfxigo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gntwkiojx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gxwvpjjpo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gneapfaya.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gyjmlupqu.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gdptjdwkj.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/ghcdjdzsc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gstiteuho.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gdsezftrq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gmtcxnzpy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/goreibpco.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/glsdtlwik.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gytmjoaeo.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/grtsfnyzc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gwzyxsciq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gvnsotljs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/guibdrmbs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gjsehalgm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvmaejata.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gdprfaefs.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/glwbcymby.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/guhtnrhxp.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gbcdckcys.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gjbzdeicm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gutrpimre.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gabxoxqjt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gedvgbojm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gzajfyats.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/ggdkttput.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gimoaqhue.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gzdnmhwxi.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gnucrpmfn.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/ghkdtfznn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gujyoormm.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gayamejst.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/glhbchfvb.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gqgkkqvqy.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/ggzgwfbjf.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/givlenlfp.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/ghrodsfns.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/ggyogwngx.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gmnyktaov.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gmpcziqcd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gwdfqnaib.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gvfdudztn.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gaubfpaui.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/grwnafkiq.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gmfmuaryi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gcrvhrefi.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gnfqhwvtc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gwukykrje.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/grhvwbxxa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/ggmvceslm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gturtzell.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gmmmviwey.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/ggmdksddg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/ginnctqeq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gugnrwkct.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gajjaevqc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gejnwtrpw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gbnecdzgi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/geulkptrj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/ggkszenig.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/giardluhw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/grpkrxlqn.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gcbhptfvj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gbziwueni.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcgdgwnuq.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gbqrpualr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtwhsirvs.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gatidswkj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/ghriemjik.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/ggtpmsuuo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/glkuamfra.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gfpdtnhem.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gfxcfhtnq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gvvvvudmq.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gewejypny.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gdkoqbzfn.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gerslrxob.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gtmvbvoyu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gmrvxwybn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gmhhjxnym.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gbulbbfhf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gxvrupwvr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gdntgngyh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gxqssmauf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gcvllukuz.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/guvlndsiv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/goazrcmpu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gvlkdsoff.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/guqromuke.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gslxaawhj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gnplnjtna.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gwpzpngcl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gsjyaflaq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gifqzdpfh.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gwylhgjsc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gjmamelun.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gsfvredue.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gmlutqxmm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gzkgmfwmd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gghhokzmh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gynpgxsja.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/godhrfuxn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gjkkocnbt.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gkgnytual.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gnaoczjvf.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gfzgjllfl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gevukqjxu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzxxqsnfx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gnxujcljx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gzejrjdki.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gacjrkcvd.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/ggkfcpryc.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/glsniuvij.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gsslwzbkc.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gycumvczr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/geolrgkqd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grctvrtcu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gwvsuivnl.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxrbaaewi.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqbfcupna.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/glfyrkgfq.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gyydbmclz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gqfsrrotj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gstsoljjj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/glssgsabj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/giafjftkb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/ggfbqhuhi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gzyxvgsyh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gzbunbnss.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gzwztrsxv.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gztklvusy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gqqmzokfx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gnwnmuxyn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gkntyobcu.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gmgpggkxg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gmzdiyqqw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/glxoqscap.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/guyezorqz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gxuaziajv.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gtjzzvnmj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/giidtfgta.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gprzskcpp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gxvlnkcky.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gzgcfvxpv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gjxoadaux.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gtopirpcf.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfbprxphz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/ggnkegxsg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gquqxhaca.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gkdpvwore.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gytovhgwm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzjmdwazm.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gccjkfpoe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gfobdwbqd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gitsxqxcq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gsvxttgkc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbrojqzhf.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpjdqfphi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzbffkihb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gzqgitpat.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdpdvufkz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gdmkzuioh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/godsalicg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gnouxcvyi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gxjmxbers.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gsrpugsqz.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/glxbqjosm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/ggntoyiid.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gvdkieetx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gediaqsbg.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/grlhdtgix.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/guoaxzrwl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gwdycznou.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gqosyckan.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gqlkiudkg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdsrpkqfg.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gnewxncsf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsyzasbxu.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gnyvjynzd.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gcorhixal.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gjpqsehdi.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gphaujpel.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/ghxqttiwn.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/glskjnber.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gzywzhykp.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gcvpsaxdf.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gspawvufv.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/giwwpawhg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gwtipyncr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/grrxhktah.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gvkthpdwu.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gldfwxcnc.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gwwdqnufe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gdjkmvoak.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gdjgqffxc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/giycbcsfb.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gtjaaqiqr.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gnxxpeseq.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gkrtcfygl.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gpgdxoqmt.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gepbbcoup.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gsbbdvxcg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gbkpxlfcf.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/grmxqfuyk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gmsacrsmi.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gsxzjeeyq.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gyiyembrx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gdgexppoe.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gucvdawdj.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gxjcvqxjq.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/guefarcxx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gqkummryb.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gekiymwxe.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gwwrgouap.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gbzlawqva.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/glfmpmyov.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gkrwiurxl.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/galcpuwwd.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gbrvevkse.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gtdngvzhy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/grdfbfxsp.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gtbssrcth.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gszqalmdx.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gtaqmpehr.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gcntjqocc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gsobgwhhi.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gazhspcrw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gozlskqwh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/geagrfwyx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gtcvhhpmi.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/guuczvjmx.sHtML


<!-- 参考信息 -->