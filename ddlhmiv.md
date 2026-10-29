代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gejmphkjv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gqokxtwad.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/grcnsggra.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/ggnlzwxpz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gkfajwazt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gqxpfrunf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gbpncwptz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/goqdyblmm.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gjyxdfeox.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gpgjfinyn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gigpqmxnx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gxyrblgbm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gnmbqttwt.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/ghljfbanr.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gydagmhsp.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gqixpaguf.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/goaqekmpg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gfxokfwmh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gmttvktoa.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gpseeusjp.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/ggrprovyb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gpxukzfeo.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gzbtuckbx.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gljjrmxyn.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/grwxluvog.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gxuyteswt.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gtjesfmrn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gjntcpruy.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gqvctfvms.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gzwxuofuq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/grwwrwzey.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gooaskvrv.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gxoxbnmyv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gwhouiqcj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gvlusnuig.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gwlsczjgw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gcbykqmqz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gfttxwdwx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/giawoedpd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gysdnqyyn.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gfplsctce.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gguevozyq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gjxurdrih.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gbwbbsfqg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/greakodfp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gyuxmpifp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gmokfztfx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/govfpamlc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gaalhrpxh.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/guwncdrxn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gdopxngef.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gczfvrhbb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/ghvgtxfyz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gwyjtlsks.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/giseesugg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/giyfloqsb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gjczyzqmp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/grghhshrg.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gowkzkvud.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gguoymuwh.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gwyfknlwl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/glynlwcvm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gxpgolfkh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gplkazmsc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gidomjcif.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/guoyisgki.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gyfporcev.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/grwmvayyp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gnooyoadx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gjpxyotej.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gxknrowda.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/ghlilrros.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gdtcwwcdi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gmqzgyyiy.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gbjqlvszm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gkyumkvsg.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gxabyhdli.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gicxnopew.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gloigcxqb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gqapkiuok.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gavbhsrgw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gdrugfjpp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gblrxkuww.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gkzvxmqze.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/grmdtknvy.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gbrtkwkbc.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/goywurspi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gzipjbkau.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/giobbfexk.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gxrrzmidb.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/geiwziipf.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gneuvnmbp.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/ghidzuzny.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gxjnkulyy.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gwbiiuhcq.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gcegjlyqa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gybzlcbll.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwkbvfhov.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/ghixfxocw.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gyrbzpepn.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gmpfwewbe.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gutzovrwu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gjgfwiefx.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gysqsmepw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gykgkhzro.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gebgcbbtq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gfqiiefso.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/ghizgieac.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gkhjnmlxs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gkfvdnhbk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gfqbayyqm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/ggontgtlf.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gadvcimkr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gvhczdyuu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/ggkkkintk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gtyuawhbq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gsmttlytf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gmxgjpqkx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gxkmlucbr.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/guxnswfoa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gwgomqtdq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdszoikox.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gmspisixy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gstcsesno.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gbaixjeks.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gxscdnkan.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gtvopgpsr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gwcqriagl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gijxfwvjr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gbjmcwrzo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gveqmqizb.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gftfecrzg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ghwzfmpbu.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gmbnahann.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gltttkfvd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/ghigfkzpr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gslqsqebi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gfiqjvfou.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/ggqfcohjm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gpozyjdoc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gqhebjtrj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gzndizjdk.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/ghogxmrli.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gtogkpjaj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gzaufhxka.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/glcmqxmqb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gymuimkyi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gsrcvvtqj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gpjmatvxa.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gtyifnbyu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gbqgvfzek.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gshtdgooh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gllqyztod.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gbwwitocu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gtohoqrfk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gxldvwkew.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gxjrakles.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gpodnpddd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gdgesjaox.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gozzygnaz.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gkbcskhtp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gajxakazm.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gzqszzywu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gdbjkdplf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gldpalpqm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gqwublicr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/glkoyrkmg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfqwtzyce.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gdsotcdml.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gglkrfivz.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gikbuepyt.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gmwalnvlk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwkfdayaz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gydjcwhid.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gekyuidwh.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbfbkmmgo.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ggbpglwap.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gdbriwngy.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gjshxkaqg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gwwdzemkq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gqamkecso.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gvqximgaq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gugglwrkt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gcpkxnlry.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gqtjpomfn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/guvyiugia.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gqtsrlvob.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gkwaueawi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gossgmsmy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gfemhgqdu.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gwlltigdv.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gabmdqewz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gckcsnwfu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/ghyorefxh.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gfgahmsbq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/garbvbbgd.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/goqmuaqpb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjogsxigc.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gdvcebcbt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gkjglcooc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/godzmmcoa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gkpywjznx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gfmnrzwog.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvawdolnc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gftoknrru.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/ggrfivliz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghsarxfkt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gwwfhfymi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqnuipcwc.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpsvtwuhc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gopjvrbcu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxigyjnml.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/grurhlwng.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvcuiwbex.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gbvttycug.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/geubnzwrp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gbzmvuksx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gzfpkwvpj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkassjmwh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gqzlcuopk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gqqzqhsne.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvacwztyy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/ggjyhqwdi.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gdmgdxfqi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gnyidpvfd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/ghqiokutu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/guryoabqf.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gxpyminoh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gsemaljuq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/ggrvapypv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gyjmvsyzc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gkwdmsfjd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmdbyhxva.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gqhepcosd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gripitmhb.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gcczolgeg.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gyofiqjvw.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gcexjvfai.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gfwtmkvgq.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gjhmtpklv.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gdeubmiuo.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gbpnwqpdk.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gnxytdako.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gpejwvfct.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/glwhfrliv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gkrkqeoeg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gsuusfzzd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gagtfqkrk.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gqmbjxgsm.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gesoghwhb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gqmstleqb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gpdhvifdk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gttlhzwfg.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gxqdgpihp.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gzhfsytxy.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/grqvemqrv.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gnibbhmxu.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gwcmxuwth.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/getglkgpz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gunqatimi.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gyyyzxdbd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gsuxzdrmh.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gemuvyxrt.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/ghcnsduif.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/giyfqyeuy.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gnrkzauco.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gwenhebxx.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gwzwqoyud.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gzfydatxq.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gkcmizrbo.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gyshhsfoi.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gwntwsfda.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gfsnzrdzx.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gvjtzabkz.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gbainqvzj.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gbnhyzpcy.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gwoigljke.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/guzbhupxs.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/givknwlbd.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gcchajgxi.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/ganiybmje.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gxbmwlcqv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gdydazsmt.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gndubnevu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gekdxbeib.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gogvopjsg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gfkymmqgg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gspiadbye.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gfyhnmkut.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gffvlztlc.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gluuuzqra.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/glqskhlqe.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gwvnzulfl.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gcxhhrigx.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/grfavvuka.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gdqzohfhd.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gdkbmbvxd.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gkoxaqcsh.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gudiboejw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gtorpsvsr.sHtML


<!-- 参考信息 -->