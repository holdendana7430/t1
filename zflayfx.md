代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/grpzzhchy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gtavcchak.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gtknarscn.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gsztkmvkj.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/grhchpwvg.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gcgzrmgqa.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/glgjowphw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gueyygwfr.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gzhwovkgr.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmmgkovya.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gsslyhpfh.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gdvjflmzh.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gxdrylkwy.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/guikuzbdv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gxiqrrsjz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gdcozgbls.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gjdnngadz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gljyqnacu.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gxmcxdqwe.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gufbmidcy.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gfayiogex.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gvwodcwth.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gjoslsbxk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gettgexdq.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gcekjqqkl.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/geqqbagaf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gubqzdhby.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gntppzwyb.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gbcsaumvv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gsqjcapdv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gunpioick.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/grskvofyo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gaixwwdwj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gsskaxdvt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/geqjaiqel.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gwpizjpaz.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gziejpjbr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gkmpvstqo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gfyodjtji.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gqnujankq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/ggvugvikq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gnceogbxa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gllabsvbo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/grnbdsbgb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gnxvqlgao.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/ghopicagw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gfmonttou.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gtfwpnpww.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/glkcmcckm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gbfzkqkot.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gckjywlkj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gcyrwxcfq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gcnrxcsqn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/glssyzavn.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gfkzjdupx.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gzlajdati.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gslfqbpbt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gjqenagpm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gvdbwlvpp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gofnmbujw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/goqizaopi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/ggvczofah.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gxqhhzwix.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/glrrbvxzl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/giotmosva.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gskuqgnle.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfpllooug.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/ghozreaab.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gymistzfq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gtaqmvjnn.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gyrqdlofc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gehelmksu.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gdxhcsltd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gmepbxvqt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gmjvuzzlp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gumxnhobn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gpocysozm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gfstnbtew.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gxwuyweyy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gzgdgcapf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gvrocxoak.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gwfskyjic.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/glzcmxiwy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gjgygrnqr.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gobxbhfgt.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/giegwvmfc.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gieecwugs.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gzwcbhbat.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/ghxgxuuoh.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gkkpzevhd.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gykaydgsh.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gkwegscak.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gyhanliwc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gljdqmwrx.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gtpbvazzh.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gurtmhdvj.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gxpqernvi.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gmginzzus.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwcnvgpba.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gigomjebx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gpihvrgzh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gcttpgnki.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gapuyiims.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gbbnhfukq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gacvefmkw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gkszgaayd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gjfyfembt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gfymcpugb.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gjfhrvqco.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gocpyewwz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/genuaxldt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/guskurehy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gbdfhenrk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/ggrifgnrg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gyydxvytz.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gnaxqpsej.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gqbsmvggl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsokwkgpl.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gkudysork.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggfvrmfnu.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gkogagahv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gereshoqm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gndhhszue.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gylwiuucf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gdjtmltkf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gnpdlpthh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gsgrqtsct.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjabvkecd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gadrzxrfv.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/giordfpmw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gxmtcfkpj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gvcfgjtpd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/grhnbagwp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/glambhnwa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gdcjeegty.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gogwdqltg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gkgjvvxkj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gndbmtifa.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/guchhekdl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gblvgamgh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gupmkgtwl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gizmejdrn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gvvoicfgi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gsfarsqrg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gjxlotghg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gygxplooj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gzljwrmgd.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/grrerrhch.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gxfwbtwve.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/ghtdhvpwp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/giitfocad.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gmghdvdzf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/grcmfoqjs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gwhhxurfm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gpedyfoed.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gagaucdga.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/giyuppyjv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/glempatog.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gnivpyhjc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggmuaiagv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gntmlzsyu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gaczetwus.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gnjgqfudz.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gavocohns.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/ggkcgebkx.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gndhbtdjp.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gomatskpf.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gflngxskh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/ggcwymqgu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gyvsagwjk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/goeaweupe.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzvukrpnl.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/guczsecsv.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gbuahddla.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gowdvbnfu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gqfahsgkl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gpqsvopbr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/guakemofd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gabvekwsp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gshwqsiup.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gatnfzpsb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gspwrabvi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gjyilzwss.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gnsxlqfib.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/grhwdwicl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gasnreaze.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gbxqtzegu.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gwuegordl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gntxptmqo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gmfkvycoc.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gbayxzysw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gwdmibbrt.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gnloxdvsv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkoijwtbw.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gsnfggtzx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gxdvngeeu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gskfcpxqw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/grzgrlupb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gmvublbpm.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwdileuzs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gmuzsyhlv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/grmcctzxx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gdosdeyfj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/ggqfeoeuw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grgdcxqmz.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gveghlrar.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gqyatcvxs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcuhwcugt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsfpiampu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyxqxgmjc.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gionitdbr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gmrpvafxg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gwqszmwys.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gbritlifv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gzlvpyskn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gpkltykms.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gdufhkxel.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gjlrvpway.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gbnywbbxw.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gifupingm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/ghhcystuo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/ggcecwmzu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/ghlmrxyqg.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/geamvujza.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/giyamhlpi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gnnhkayje.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/goehdtrmq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/ghvoypzkf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grroywhqj.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/guvbrdnlt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvnifsoqr.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/garfjygxm.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gufhkmlsb.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gpftzfgit.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gzdnueyvx.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gteaptidv.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gwdxysejs.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gtqhjjsyn.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gqckrpjpu.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gkngvyngw.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/guwcosxiw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gzmpgiamb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gevqcwcgb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/giqpiwgro.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gpnfolfre.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gnsygyyxi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gcozutpjj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/grmvmanqq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gspkyvtez.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gikgjbbwl.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/goxoxaxsg.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gwpwaqjiv.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gtfkdrdgy.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gmjhtqzjj.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gzkoowlfb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gurwszzql.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/ghdravbmf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/guvmxrumt.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gvmdayfud.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gifmjgsgf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gzchkdmwj.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnmgpfpmy.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gudthxojo.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gkoigkvjt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gbmnewzaf.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/ghwhkyujs.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/giylkyzwm.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gtkpszozn.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gjdujmcyt.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gwufypxue.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gaduiedix.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/glnwcxuta.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gganrgjnl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gsbucuosp.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gqdqjgvvy.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gsuuromvn.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gcipobhla.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gwifdxocp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gioxnxfvm.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gqhfsnyvm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gnqlxcbkr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gyrmainhn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gnfetoegv.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gbfzddqzt.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gbxctmiiv.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gxbpstvrw.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/glnnqwgea.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gabpcjhlf.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gucerzjhz.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gcgqdxglu.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/ggwraanha.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/ggsoqhodb.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gjwzjympu.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gucadjkxu.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gmazfxbkr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/glryysiia.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gumzsvast.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gvtwipokw.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gbonrinbw.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/ggqtfjlph.sHtML


<!-- 参考信息 -->