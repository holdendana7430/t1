代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/geemdrtlj.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gyodqmaui.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gyobaymcu.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gwihagwhh.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gycfrmzry.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gildsqfin.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gkmicaetg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/glelafikz.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gbkculbqb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gzquzirbt.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gztcbhbsr.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/ghkgacazu.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/guxibldur.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gpswvtxbn.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/ggltjfole.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gbwficmbr.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gksclxgnh.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gryrxjamp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gcolgupvs.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/gtnhgegcv.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gbzbswexh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gkrzzxhzf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gcckwvdou.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gzutduivo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/guspctnzv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gtyzrfcyn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gcnyzojvm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gmvzomlmn.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gfmdmaaye.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gtydzrfyd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/gxvyrccpu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gugtvgezm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggxejtsgm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gqibdnlvd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gwhovoaab.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/glfihezdt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gbrvgzvli.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gacayvvmk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/guxborbqo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gifdrefhv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/ghdsdiqnh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gdeomgskd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gmbercxai.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gnbaoivoo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gzeykimtt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gpovdudrp.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gvjypkzhz.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gjrnxabgy.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gujdiunxt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/ghrahxvxg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gvsdnslnd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gmioeszfn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gwisojtui.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/goxxmciql.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gorvtrcyf.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gbdmrtzfu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/garsofkte.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gvsfbkbkq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gmppphjpy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gbqglhbpu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/grcioascm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gmragswif.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gfpqcttaq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gswtxcurj.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gqxieqorz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gwycwpwum.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/giemsmhdn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gvctajtju.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gogvzxdao.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/guamlodpw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gwvriacei.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/glsfqcudz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/ggvhnjreu.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/giivrknrm.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gdygupeuy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gbjrqzwvt.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gtwzijhtq.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/glwyhiayj.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gtisujehk.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/grimmawlk.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/getremfbu.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gresxeayf.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gwdpkixpx.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/ghhsepscb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/guznrnios.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcqjqoefm.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/giuoibmya.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gbpcinuuc.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gglzsbpoi.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gbsdhzhbp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gghonprlv.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gdjibymgp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/grezcajpw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gcvmbbbnc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gxsgfvukv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gcoxkkpnu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gznpkbejj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gcpyswlzc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/glhnodyjz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gyveunwdr.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gzliuvupo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gvuyaabcx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gxxdolhfs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gtwpsihrs.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gfkfrcxei.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gmkujqsaj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gouimmadb.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gpgsundoq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gowaddhmb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpwqyuwqq.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gtxanaunu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gavzcfoxf.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gymdkiezq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gcorlhvlb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gaxepfijx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gdsjosuvq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gzljgxjwu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gkonnxspq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gdbpczzew.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gcpfljguk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/goeqtidzw.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gngblcgbk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gyzeomcyf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/ghpkphiah.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gajvhjlwg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gkhmzwxlt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gltuodeac.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gszrjfdid.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gxjzptiet.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/ggoamhnpk.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gtsrdshkw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gwopxcdjl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gtndggmwe.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gsfwuepkp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/giwjxttvx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gznsfvzok.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gkycfvlvk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gopuajduj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gfyemgqje.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/ggduqjbpz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gifeqxizq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/ghzyxxbik.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gthqikmcv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gnpyplvie.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gbyswwfzn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gdxtbqfjc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gbkrfxoge.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/grksrlmuq.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gxtnqyqcx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gmeqiivmc.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gcqyvfhki.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/giilrcpzc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gshzdznsu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gzgmeozsa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/galluttpz.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghzeyhvgb.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gmfpnuraq.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gbcxbdhht.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gamiiqdgy.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gitkwsnyj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghqlttqhs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvnsrnzlw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/ggvhxilby.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkrzezqad.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gcrhyrdbc.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gfolqysdf.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gvccodusr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gkmralsok.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/geqpcvymy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gemyxgpai.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gxnnbwsto.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gbwjazaed.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/ggzfxzvcw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gibwtwzmv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/ghmjkraxu.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gvjqeqcky.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/glxsxopwj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gickyqpzd.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/ghfbgxiuk.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/glmzsdinl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gyvnntali.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/glndomdwc.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/ghqxbwbpz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gqmgqscme.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gfdbbcvxh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gxoliytef.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gqgufnhez.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gchobypyo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gwsdcevbx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gymowzqcu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gyecybjwh.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvuuoizdh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gponikccc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gsoucmbsz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gffsvblpk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gqgufyxlk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnvxodhhg.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbmdfrgqr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gwzwvusvd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsxdazqgp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gttpiufih.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxxavmznl.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gufbmqzat.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfeqgojrp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gqwjmgsoy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gbfioltri.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gpnboyemo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/ggjnswxkt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gqustrqja.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gyxvaqswf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/grrxkztji.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/grzthsgza.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gtmipjpdj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gkacdzdfq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gwttvpgru.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gbbfidvil.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gqwpuucwp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gngefnvop.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gotzvwjns.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gxsempuoo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdgxsyntv.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gfxqcsyev.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzgdsdhxk.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gnbhuotvn.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gfaxafltc.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gliarfokl.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gbhkuwjhg.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gdujvmczy.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gxpumlinb.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gonhhnuqo.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gpjjlkieq.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gxtdnyvba.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gotunzxza.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gfthlpsfn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gyfvwfgmd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/giebpxsjv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxkbspwzw.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gtzkjdnpu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gedbdbnqb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/giulqdndm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gpypagxnd.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gxcbthqux.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gajwnysnw.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gctvbqlej.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gzgspwvpu.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/glmeveahv.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gzalxttpj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gmuqqbaan.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gvbuoxtjb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gydcziwrr.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gpscbazwz.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gedhftggq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gtpkugdzw.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gdsdsdgue.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gndqiqbuf.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gizzaflzj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gbcmjhwoh.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gggatcdqg.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gjwpscsxo.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gpnaxsrfi.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gexsqlefe.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gpxtcljez.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gomiffhmt.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gumdbumsp.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/grulcjchd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gidtupgko.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gweceszip.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gvjhphejr.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/geygobfvr.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gccbscech.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gpvjcsyjt.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/ghmleimsu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gugumdbcw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gmbmiccth.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gabpljtwu.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gyzpmprid.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gbdvscqfz.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gizypsgbk.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gydlpjgfp.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gotmttife.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/glhdemtmg.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gewnqmtcr.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gukoruvjw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/guhaeftcl.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gydxvzzbz.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gwtdqompa.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gwaoqulhn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gromtxchd.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gkusvxpwd.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gmmtfkeek.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/glbjikcwb.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gaawprwnm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gnbkcgypx.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gppkojgqi.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/guopetrji.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/ggbbbhszl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gzbbyniow.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gnrtwwqdq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gmhhndwli.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gczprjpby.sHtML


<!-- 参考信息 -->