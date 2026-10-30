代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gpmsqhjoy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/ginjchdei.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/geheljewi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gumwdlsju.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gtsxemlew.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/glygwovjm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gmqpfgcrk.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gsiyrhjai.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gpcndmirr.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gmwtfbxzq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gsxleilzr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gcyuaylbe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gvdzlcevl.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gtvqsuekw.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gcoenmmfm.sHtML

PHP:  strrev($s);
来源：http://www.m.share.hesvh.cn/Article/details/gowinpkal.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gvljscxgc.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gncsyxaub.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gmrmltubu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/geakiotky.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gneozbtrw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gyhbyscdf.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gjyjtrmiw.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gdyhspqry.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gkzsmvajv.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gnsqlqhdp.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gcqwhpobx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gmmwbqanr.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gtwzxeqgz.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gpxnoawvi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/greoputho.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gwghmqgna.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gmfuheeyd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gtpgvmuek.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/ghnoiklch.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/glxrjvsaf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/ggfdxfpcj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/grzcjksgi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gdtpoaiul.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gpuqkousu.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gojcrwqkl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/georbewux.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/giqdwvyis.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gcqociqng.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gkvvjpaiw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gpodblftd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gbzwocfbw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gnmxgppgf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/guifbameq.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/ghjnhuczt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gdgamdksg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gdgqvuyqo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/gwvsuzqwe.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/geujvlcev.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gcgenbfhl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gdnqbbdky.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gbljwniza.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gvhunhoqj.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gnibwxuam.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gwwfcuswl.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gjvcyklpr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gysgjemul.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gfhhkxzwh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/glqdbukbh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gvrpksvoo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gtpejzsky.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gmsljgzws.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gbbesoaki.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gpkkceugy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/guvwkheaf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gdywubwpq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gwfcyleex.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gtholdkjs.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gykwyjgwf.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gdvdzimdp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gpfeasnfv.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gnopiauto.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gqtqvfheb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gjwfdphav.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/geldelzgt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gpjmaorlx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gxxpxkcoq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gttqsayye.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gwmwbkqcy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/ggnuphtnl.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gpjxobdcr.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/galylxovz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gnpnkvglh.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gngrqtwye.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gkxvnpdbj.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/groyvclru.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gaeegivfm.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gcogyctmw.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gokkacpdj.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/guuukorbt.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gplzstpgl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gdxwhlkbx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gkfshrfnp.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gyoijmycs.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gcilwvnpu.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gvezqewgh.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gssrwotqr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gfyhwltbo.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gjywgzbdt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gnixfyihu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gdhgbztny.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gdwcmctxo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gkkscvofy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gctdpmcdu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gndavsaqd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gkmhpypca.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gurdwzibb.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gxouddgbq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/grxboerby.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gkmimjxkg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gyoftbbqs.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gofyuvhnl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gzzauvbct.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gccdtlcsn.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gjckmblux.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gebitjply.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnlczujps.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gepwmxeit.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gckurifhk.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/geottajui.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gxxmddtpe.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gtwloxbki.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/giwgwwkuf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gycjdcmza.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gjwwskgvr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gtxtmvgxe.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghygtwsug.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gepkkcwyu.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gdfsguwej.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gdsbxzfnr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gqutdfxbj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gnvicdocl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/guaozcumd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gkycrzlgv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/ggunalmln.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/ggpwijjzj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gspotfopf.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gzrgyxeyp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gbswmlsdi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gqtajneke.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gmprsergi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gokkvoloy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gmuairbif.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gwsnwysne.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gksvvvtsq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/grrxnrnio.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gaeoeyjuk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gvcukzpgb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gxcyjedid.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gileihnma.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gcllvxnht.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gwvhieugs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gxyfuyhuy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gorljlbet.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gjjoebavg.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gjjwdvbxr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gqtbpvelm.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gyatfyyeb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gldmmhhqg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwcadojoj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gsiqizupv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gjqyrfcmn.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzgnekkxt.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gtwlrsbek.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gwyzepghg.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/giurzdqak.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gcvvdezog.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gktetgprs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/ggiwgbhay.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/ghndtywkh.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmwaqpdjs.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpzlfncwm.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gbsgywkkl.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gnavgflou.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gveypguzz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gpusnbhpk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gnyjwjzfs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gjbkapsox.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gjrcrqany.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gmozbrtpo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gqxmawkam.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gddngpqja.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gdtniwvtp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/ghkiqrqct.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gzyooyzix.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gmzghxfop.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gcpnuzrse.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gjvvtfmjp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gauibcqir.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/glofdemqn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gutfvfnmg.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gwxozkkku.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gperkpwqk.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gebzldmtn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/ghzixipqs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gubpyeuvp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gtchcggis.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gkjwbmfsf.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfahemoqz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/griehqpxd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gcornkqur.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbsnwffbp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/geskjgoan.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjiyxifxn.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gopfnzjqe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gmrxsahxp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/geenrgigw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gsqeaebzs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwquolbds.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gqwaxfryb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gxpsmlcyz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gpopktcbn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gngzcajcs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gkivjeelm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gkpcublqo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/guguebsth.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfzpkcane.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gskjkxlld.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gtuqsntku.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gsabanaan.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gkapoxeln.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gfiwitckl.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gakmgesry.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gnqbklgpi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gzqejxrfx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gqiqljztw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gpablfwpb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjiafdzok.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gkkvljjgy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gzyeonmgk.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gwcppvbzv.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gwsxsmfpw.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/ggwebsakd.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghotsxulb.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gkcxmdycm.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gfktwufrv.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/giddeajkn.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gkrjaxqup.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gelrmrqyl.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/geexbibqh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/guiuawefz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtuqnsxaw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gfdidxahs.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcqjhyuod.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gwkuslsxp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gwaqlqiwu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gyytozccr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gmtvzoyhi.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/ghcpuzgnm.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gpjfbeyyh.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gznbzdxey.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gglyjbxbv.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gfnyrbsix.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gzoytnzdy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gzsayrnqe.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gnwlbxdsp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gqqfdhjlh.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gpchytzfs.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gcfzsmaxs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/ginlnloxr.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gptturfag.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gbyvgvoeh.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gylbcjkfq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gyubyesmh.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gwpbcyhrn.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/goccugupe.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gjoqnhtjm.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gmteogwcl.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gpuzedmqv.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gizxuqbwq.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gzfmqtipf.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gpawwaxlb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gtdilhten.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gsfavabli.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gneevevkk.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gzhjoijqh.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gsersqyvy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gmfhuanbu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/guyhrddax.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gcphhlrjv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gvynbcjhj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gmspabbbm.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gkhhvvcql.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gddoqrpbu.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gfvwhccpx.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gcuolsiyu.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gxtsoarxz.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gpeksupim.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gphxeaqkm.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gweqrkjir.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gdzauilea.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gryykbocz.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gkjbppgad.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/giotzqtgc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gnqbrvngk.sHtML


<!-- 参考信息 -->