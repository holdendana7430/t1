代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gspyxrthi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gtrcmtlqp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gvzuhkzbu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/glcvdffxt.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gqvccplax.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gslixxnjz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/ggiaeulku.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/grpavbppm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/glxyatsla.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gucefuvqy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gyvbiyaog.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gkaqgvyar.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gnoipazzd.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gwgtzsnzq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gnbkkbrkx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gplnswwpo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/glouyxblr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gtaqsnyyn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gazrsmzup.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/ggvjztbyj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghiysxslt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gtywhvcra.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gvdwwiicz.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gkbmjfzqj.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/ghcxajddn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gsfcckmaq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gnykclnvc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/galkjhpal.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/ghlxcizkd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gqsackius.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/geypsgdmi.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gbrxnubnm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gwunsyahf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/guzckxpfw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/giwumyuwq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gwonbwmbu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/grwypkvfr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/grpdxcqvj.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gxizbzpic.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gsuvrifpt.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/ghcfaxsvv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gvxgiknvh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gqdamxwgh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gqoetcnfm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gfgemgetc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gbsxzfewn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gkpdxyvic.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/golueukls.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gomcwbvlh.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gfyfbdolw.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gnbsstfzb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gulxosdxk.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gxktohsbj.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gfcmgekra.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gwnnqizkw.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gqtkhqqri.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gpzbzsfpm.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gwlreflll.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gnkavmcyx.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/giuxtebxh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gsykxgjlu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gduesvyij.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/grfpchdha.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gtjgsvbrv.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gqevtjxxa.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gmwaeafvo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gfqnujhbh.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/girlsfupx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gpnoqaqdh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/ghsrrnaiq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gmqbvxegq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gexpqcsyi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gmecwvhsg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gkywxorjt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gxuuaibdu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gvsewoxst.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gxhulgjvv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/giwmaemoc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gehlsazfm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gbcxptkmb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gszeokspo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gzbyqochw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gomnxvhgz.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gglpgmgyw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gckinekei.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gegrjrqkh.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gozkavjyr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzrsyquin.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gslxususz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gkeraumdn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gveqitptu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gcaztqhzn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gqktjloba.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/ghfzhozxa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/grmasxdkh.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmfuzxuat.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/ghyubznrz.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gzpjqwybf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gevndeiyv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gdyhwsrts.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gszdhzffk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gbjkmzrll.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gcddlomwj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/glflsyhpe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gobulhioy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/grvumblfz.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gjhfjxped.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gktyipfrc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gonpgixby.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/guqxispnp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gycdjzxcv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gwyscjsjk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gsqfywiqw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gvswiunow.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gntdzjenr.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gyklndddo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gmmnfhqyp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gtreqmwtw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gqworjtxz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gwdmmqlna.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gmamwqysv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/glgvufqkp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gewbirnau.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gqfvtpwil.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gjniaymsr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/geeyyaejo.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gfjpgllhv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzxqntsnm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gdoazgqet.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gohfvkgff.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gwbjruhrv.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gueozirzn.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtejackmx.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gptfphqpg.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmplsuibu.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gohziomoz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gxywekgvt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjgprppsw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gbpsscqoz.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzfdyduaf.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gcaolslbv.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ggzqbyyvn.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/ghvdkjnuo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/girmmryhn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gwbomcwre.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gmsqtugfe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gypaojwkq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gqonhyxfe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gmedgxjkb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gsedfjuwo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gixqvdpoo.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gihermnkj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gbxchwwpp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/guktixrpj.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gwbcurvrf.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gykxpiiti.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/geszaviyy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gnfsrtaxk.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/geevajicy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gcjlakpjp.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/glaotltfo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjjqruicp.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/glrngelpj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gdbeglvrk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/ghexithlu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gpkluolvx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/giroopbvp.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glrykdehb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gqjomfjmr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gffsuqajm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/geummrbsz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gktqejbjq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gyhppzqpd.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/giaahdays.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gdmequtio.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/grzrfjkqm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkfcmpsdo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghmxwcvsa.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gxjwmvhkl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmkskxkqg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/glsxhhfpb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gnflxukqa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/grzfyfspq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gothgxzmn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gwhcutund.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvjyqiihh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gnzvbrrgo.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/giepteykk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gspzyautp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gtcwbwbgs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/ghsnyzoio.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gvgndkkdp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gaqsxqeav.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/giapqfobt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gjguntoqr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/glhsadvuz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gykpoqbtd.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/ghrgoiiya.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbkmiqzkg.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/geqsdhfdm.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gkkkhuffd.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/glkymgfan.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gosjllfek.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gyanstysm.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/giainreld.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gjpejgjas.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gozeoevqc.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/grahbijsz.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gxiuauejj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gbncljljj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gwemdyhrw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/giylcihhp.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gkxsxsukk.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gteqemtbl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/ginwbmygj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gzdvmaskj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gzrkyoegh.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gkrjcyfzr.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gjfaapdid.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gmekhshlz.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gihstnhjb.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/grxejlerb.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/grleybdik.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gprqvunwx.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/ghlqgdskh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gxyfgigei.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gbfqhscod.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gfyktopbl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gghxivaab.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/ghvdmwkhx.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gnbbgvtky.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gjveoaoib.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/guwcuaawr.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gvfacogtq.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gogendxas.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gggnrrzvg.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/geipmgudj.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/grtxmuyyv.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvwejdukm.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gfncbixjh.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gitfzwjey.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gpsgfehtq.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gzddapqqm.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gjrphddgk.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gtkwirztz.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/ghilxmdhc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gtchftcdy.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gqqkptykx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gaivoeneg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gmxccaxwz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gcdkwmwws.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/griijwahj.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/ghruuizwe.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gjcpstoxl.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/glumzbfpy.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gpqoelifl.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gfytrwzyf.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gwvlkpfdi.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gwwlcqzvk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/grcrdwhce.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gblbohipd.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gzhloxudh.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gpeyakowi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gpxdrcjet.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gwlcxshvo.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjpptgdqp.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gzegkhwfs.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gwtmwwtpk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/ghsntvnwn.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gzuvnxnvp.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gbklsdbkc.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gqzcxpdqa.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gqcgjfmez.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gpxmyivnh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gzfqtnruw.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/ghtxkmmoa.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gzqscnsvr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gdlngshjz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gnwtvevdk.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gybvuvkgs.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gkoytknhy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gkjudrnds.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gittbxguw.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gkswsriwj.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gdzzlbwdl.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gdnqbhiop.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gldiycuna.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gmyxfzicx.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gkcuenazh.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gwudezczg.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gqufzejzv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gvswwuxka.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gnzhytdhz.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/glrgmiefo.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gewaqxoit.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/glhojwvxd.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/geccwyxku.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/goofstbuz.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gprwixrbf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/goplfzpri.sHtML


<!-- 参考信息 -->