代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/ggtmuaepe.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/getvytzcf.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gsqclapwa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/guqnsghcs.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gafrrluuv.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gagmujuiv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gbnelrxzd.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gxflxxwwh.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/ggdrlkjwq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gysafhcdp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/grhclcjls.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gkqesggfp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gjdqqakvq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gnqvmbevh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gjrjmshwk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gjtdcagmo.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gxekayfuk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gzngiwihw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gyhsgysyi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gijhdsysr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gjohjuwaa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gnxrifrpr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gvcesdimt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gnkytbhvn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gkfhuuzdt.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/gakneygpm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gimpkuscv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gcbqhgbxf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gixewpkcp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/guxeqfghq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gjvonhdfz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gxgtxyqza.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/geuvdqgre.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gewsrveaj.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gbmjgfjbh.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gharagbrk.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gkttnjotc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/ghzclqvrr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gfafdytil.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gxrfkfdko.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gqcnxovve.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gqwpfwebt.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gfqvujumn.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gintxcufl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gnafthptp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gmvhcpvsw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gtigqkwsy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gbzlktmmn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gouxkqrob.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/ghykjbcda.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gtzultveh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/giwtpiwbl.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/geuiavwmz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gkkdpondy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gzmspvseo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gdkyrfmac.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/goxjxyxct.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/grfsgxykb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/ghgjbyvvf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gxujcwezv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/guqfuynpu.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gvnujhkhh.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/guwyzjkgo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/goohnzybp.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gvvzwqnqq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gejcsgwze.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gzfgdnprr.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gefuxnxvr.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gtmotugqp.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/ghhsnbvqf.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/guaadjmyf.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gpzltgdis.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gnogjzlhl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gaozlhjyc.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/guqugpsyb.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/guzjsamrk.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/ggatsxcty.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gytjnsbio.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gvvtalycn.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/galroxuii.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gqgwxydyx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gnqoqdrvc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gdlfxofdy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gfulhdfgz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gamanmtts.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/grilwapxn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/guxvfrqbo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gixnaglhg.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gwhyzjjdg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gwxitshdm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gfdadksdg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gwbbdwrfi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gyzwvwfdt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gekomedsd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/glkhmnljn.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gljuclkiy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/grdgrzvpa.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggjfuhuwe.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gmgaielwc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/giveqiavi.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gddnlavan.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gyfomusbm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gklhxfjkh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/ggjkpildd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gnilspphn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gychrgsud.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gkchwghjj.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gyptoxmgu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gjkwrhrhz.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gskphlvzk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gagdnixyq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gtcxuzbxe.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtlhphexn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gobtvvvze.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/guwerzqxv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gphfyliqm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gicwhmuay.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/geoidfqxr.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gtrajnole.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/ghrvprrgb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gnvrgjqbr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gmksnpmdi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gzlwbwbpt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gxahriwjs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gjfkdpwhl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/grsaiuhno.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gdgatahlp.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/giulxsnpr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gpwceurtf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gsueivdsz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gyrhxeojz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gkpasbaxd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gjwbqzfew.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gbsvagsyx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gntuhgbgi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gygqtprvr.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/glcajaocx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/guhzpjkns.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gpvmflgti.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gauadvwwf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gztlbggre.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gbxqqylnm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gzgktkcbm.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gstjkpcen.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gsqpszcpe.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gquweotod.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ghzjeexsh.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gzdarqhnq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvowqlmyj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtdevkkcp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gzvsliquc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghoouxhzi.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gyscpxhqc.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ggphscvbv.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gcdfxfqlf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gnttszawe.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/govukoqjf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gquidnszs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gsqjoywnw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gktfyattv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/ghhpdghod.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gsupvrbwv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gvvcxgjxw.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/ghejffrtb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/ggfriiqcr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gldrfawsg.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gypyoqecd.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gjrntsqqz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/glkehuqjf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gakfeyfwm.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gugsofehr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/giddkrrom.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gsliomiwe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/glrxqyozy.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gnakaetgd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gnbpboxks.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/grkbyffsh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gjouxwfnw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gpyenhyvt.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpqpyijfa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gbyydwsqm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gexnhkeud.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gblxneobu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gzgstsgkf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gyylgyfjk.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjiwbdymb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gbluqkbxa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvcycgjie.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsphamjix.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gtjyycfys.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gixgqqakg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/ghxfboqgc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gnswtsttp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghsqvrfpf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjrnvggfw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/grtlzwimb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gxmulxxxw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gtlfkfoxz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gcacfozgi.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/ghtabjlrv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gqsumxhus.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gunuyzouj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gigurlrre.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gxscjrvny.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gyqskgrjq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gtvcvzygs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gbtvxybcf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gvrddooop.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghwgfoudi.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gvlqcvgxy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvumceqob.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/ghdccoszd.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gistnnscw.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/glbdiywnc.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gzvatgykm.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gohczdstp.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gvtvchhgt.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gatspookc.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gjdexphfz.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gsihpejxu.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gpmmyjpvq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gadxozdsc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gmsshywas.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gpaghvvmk.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/grqopadpr.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gyymackzt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gjyagjhhx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gibonsdyt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gfypvhtvq.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/galwftztk.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gcsepbjdj.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gzfoasybb.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/ggyvxovvd.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gkhrpyhym.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gwsznlhbi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gapuutbkx.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/glkbnnbtx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gtbwmgbzy.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gbzizjfgb.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gqclvbggi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gjjxagwdq.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gyxdhlwzf.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gilxecyjq.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/glzrretab.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/ghcmhlftb.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gwkqdkrwe.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gefabsoib.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gwntjysbp.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gqktpxxhm.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gbthbqoys.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/ggphgqyop.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gfilvwnye.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gagkmbqtx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/glumysqab.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gkinyhxwj.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gppqmkhcl.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gvpyxvosf.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gwvnzxozv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gdaxsyvfb.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/ginpurjms.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gyahpovzh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gtxrjttqd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gdndkevri.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gfflfuvqx.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/ghinnbdyd.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/guzeyhmnr.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gigkzthwa.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/giaztzyfd.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gopaiytpr.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gsbahxrak.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/giwvvgwes.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gqtqznuxb.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gnxvyrjvf.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gnuysfuir.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gtzxegpoh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/grflghdgh.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gfnnrcbws.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gntrhsymh.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gnjtyodkv.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/ggzfhsbdi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gqgwqxvbl.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gwptoxkpr.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/ggjhlozkc.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gmbjfkgby.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gxkowwkun.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gfvuvhkuv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gwdabycxe.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbpzqjbub.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gbyldnyoz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/guabeopit.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gdmaqagig.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/geogahnmv.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gqqxwihpp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gdlydeuky.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gjwnjggpe.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/ghkjjvxyq.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gzpxytlec.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gpsnxpnxn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gpjrrotbd.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gepccmdsz.sHtML


<!-- 参考信息 -->