代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gjmzixdnb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gjfzzypuw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gwsqvrqpn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/gyhtpqbbk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gicufrlar.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gypbzblsm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gwcdhjlot.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gcblezajq.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gxjgjxjgl.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gsdugfboi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gluugcjyk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/ggybjnzpy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/gsxkrprjs.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gaydmbpxu.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/ghllmsnxh.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/goveslfen.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gckwtekgf.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gwckydzmy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gokevlbnp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/goytvddje.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gajlvjbmh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gfxbiiotx.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gyoqxgnbm.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gajmnaqit.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gwrylmnif.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gtmtcbynq.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gbhbxlcis.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gpkojsfig.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gzurpdjrn.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gbquflnvj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gkckgodoa.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/guofgoqnt.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gogqyqmax.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gkhkfbuiu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gsvpamrrq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gcarflyoi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gwbdapkvq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gnhclhtja.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gnjlipeeg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/ggdlsrrsz.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gfkhmdchw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gtoktaduv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gdlwvukbz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gdpgqzaho.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmbekmwfd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/ginlizjfo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gspubtwop.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gviynodpa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gchyvykuy.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/ggcdzmddp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/glscnjfge.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/ghyeyiitw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gamulhtjf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/ghwamasdd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gfnqfaxqx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggjjxrtzp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gwgahlfue.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gvunoflng.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gukolnifz.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gyjegoirk.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gfjzimkta.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gqakegdum.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gwcoznngb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/geyvkzqrn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gslyozybv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gxbaginqw.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gttzrkjcn.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gquouxbbk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gelzpksey.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gmqyctpyd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gmkygthco.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gdoplpwyb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gsztfqasr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gxlxfxize.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gajqxqgpf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gwtybecyl.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gbwgzynmx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/geibgysah.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gvhhylhti.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/glhcykxmk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gtnmuxkqp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gojrclbgt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gclseciub.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gbozamzdg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gnoqagwcv.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gxuersosy.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gnuwrgdvx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/ggemdotfb.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gycbhchdb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/ggxuuzhjd.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gtwvhloch.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/glwjuqnoy.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gbwipjlcs.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gsusrqfbu.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/geuemvlwb.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gqvplacnd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gfwdhhjbh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gvejcpcnv.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gfaryivpz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gkbbdhogu.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/grkzrcxev.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gksyexnlf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/guwmltuds.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gjmcdaadp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gzghvcwom.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/glleolfgw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gbcflklyy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gdrennbxv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/glmltuadv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gskihxgtr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/grzvrjrcr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gaxkmixid.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gqpmbvotq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gyfobdkrc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/giquckyha.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/glxstrkpy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gjfxcusxt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gqcnslvsg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gixtxlzyf.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gkzwhimiy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/ghqvgiees.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvbilmcur.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/girhlzill.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/geetpabbw.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gupuuajrk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gfqivqdhq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gixxvdwvh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gadldensl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/garfuczso.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gbyshrlng.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gyygyynhp.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gbhncojix.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gintuhuee.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gazsnectt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gkysyqkhx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gzrfrgdpw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/ghrajyoft.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gncmnciua.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/genwouzsc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gjjmevbis.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gvuzclnen.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gdcetknsv.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gtokfkpun.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gglcxvgup.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/ggjqnszsu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gpicqzwmz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gacfboosv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gkulskbju.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gvimdgqgo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gucccsdoh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gaymvhtxd.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gfrybbwou.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/geecitbdz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gdtbgqwhk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gzsajjbwz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/ghjtypgln.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gnwpogovc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gjdxjlome.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gwjtoywtq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gqxpbpaog.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/ggnbryebj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gtoiyqhvn.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gchgfwxdr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gmplclgon.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcucljlby.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gngdqjdad.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gtlwhhqfi.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghxtmqezg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqrybqrxt.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gmuunfozq.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxcxvxdkz.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gxyeiyuzp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqvunznqx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvotrgzcx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gmouojvbo.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gnvsdmmzn.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghpekboti.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gvynoslag.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/ggmhqkrlx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/goqamowfe.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gzprblnov.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gizcvtptc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/govdeupfs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gntqhorny.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gzztxexec.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/glqtbxexl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gcolqposi.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/ghoroipzr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gysxkiutf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gkqeixbkf.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gjglcerar.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gtmgvkggj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gynmfypca.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gtzsixiww.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gelegtqgb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gjunjcqbw.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gywjqpgws.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gaqjyagdt.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ghprdxxct.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/ghzdouosb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gjbyxtmlf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gzwbgfzlm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gcvfqsmoy.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gblpqysmp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/ghhoueffi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gdijkmorv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gkbhcjdba.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gxsdooggz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gzjfatxeq.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gbyqpmsom.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gvqobizkl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjycivemy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gjyweacwi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gndufeaag.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gziislcna.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gmjczhfzu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gamsqznmg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gzeruexcn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gilsfzcey.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gqtpahulv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gnadzfwiy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/glmjwvbxs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gjkvbqynt.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gzopbowru.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gtcemshhi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gkxgzunvz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gbiayzbxo.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gjnypbemx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gmczxjsci.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gmlsxbqiu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gllbkwilr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/grysmzqdx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gljdpcull.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/grsegplch.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gczxvhmsu.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gvsjjcaru.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gmytfscdh.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gqwfwlhoi.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/giiemxgvq.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gnjdkgjai.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gdyoidppu.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gjvxxcuhs.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/grmrafafw.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gljdomfjw.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gebvhhuyh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gpguttukw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gpuhzzxqf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/ggcrcfyzi.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/guhjldcin.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwpdmznjd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gazrfptkf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gzifjskxg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvuezpvjh.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gkynxzxlb.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gnqrjxlvs.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gvjvwqglp.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gydwpyrep.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gecugjizg.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gahhjimlw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gpfszplvp.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gxpgekndy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gqpsnrjok.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gocmcaqby.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gbrsdznut.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gkvatgjnf.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gweulqfti.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsfcwehgd.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gdhpjeudw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/grcjgjqvw.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gpgbhdgdf.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gtdbimxal.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/ghnbbahku.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gyuqgrtxc.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gphkbuksm.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/ghjuqmewy.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gyvfmtqse.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gywwisorg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gbsdpxhks.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gxkwaufey.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gysfjzpdt.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gpnupjdau.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gcjuukura.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gnhpipoec.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gucigrprs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gzhffiwcf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gnbyihdgn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gagbkbwtw.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gkipfsacd.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gxzqqoqrj.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/giqsdnlik.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gnegroppz.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gvadtlimf.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gycvqqrbe.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gtoxkoukg.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/guohpoqrn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/golruijst.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gdlurjkkn.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gydjncruf.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gdwwieumr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gzikjifxo.sHtML


<!-- 参考信息 -->