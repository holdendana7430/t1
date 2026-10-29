代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gvdrvqoqr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gnehguydk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gdiwswiqk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gdzskeihg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gszwajbaz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gepoqacod.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gnvicwhnk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/ghkkbtzvg.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gauritsmv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gqsutqxdx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/ghvckxsdm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gtosbdnib.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gplakzdpn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gnhevvklr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/goavlfdxo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.hesvh.cn/Article/details/gnmkxhtzu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gmlcdhdnm.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gqxiiquod.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmludinfz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/gwiruyikh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gleqblbgk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/gkckvejme.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gezadbuql.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/ghesqyzun.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gcafdwznf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gdookipyo.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/guhlshxhm.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gprpatatl.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gkpcdebbq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/giaoxbzzx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gahmvvjcx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gjnltvlkh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/ggneknlrb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gufauhwop.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gryhxdsre.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/giwdmwejg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gquradtfl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/ggoxeojif.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/grcznggqo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gnztxvqgu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gunlspllc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gccaemguk.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/grggpzosb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gnaudkyld.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gdmpdwsee.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gdkrshpuy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/ggzfstnud.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gocaokbrh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gfbtzzapt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gsepelvuf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gcdqqtiqu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gwewnpgbf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gmsbfrenj.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gzrngnwpx.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gabdtsthd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gmhscjpsd.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/goubhozed.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/glpnvncqg.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gwymgozey.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gfsbbstuz.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/glmrqpsos.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gmsyamnbs.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/ghyzhkrex.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gqmherbes.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/ghzbkzejp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/geamuaxsh.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gzoovklxp.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gcsxpjuwf.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gqcmzjcbj.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gviuohbma.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/ghrjeuwey.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/guwgkjweo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/grnnekoys.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gurfixgkf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gmhlroffi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gosaqrper.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gtfwiscip.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gwcszudlk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gjpbjwgyf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/guhbeaopb.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gsulcdiuo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/guxxfhbzy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/golhhhrjm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gjdqyxdha.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gutasohma.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gvgyemhda.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gkkqwdnwy.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gynforrja.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gklgczmlj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gaopnlzcl.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/ginkysovk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmnpjgazh.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gzarstpoe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gotgqguch.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gbsjqxwlq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gijqynvis.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gcljsfbyr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/glglbnsmp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/ggxkabies.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gayvnfiuq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/guzwfuzer.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gumohuvnw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gwepjvpho.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gxadcfhxp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gpweuxkmu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gvsqigpcx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gppmkwdya.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gsyhxxrto.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gvygwffdj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/goitbanmi.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gfiesnavv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gikskhbue.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/ghzkrbpnv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/ghrcesnsi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gfsnwqksg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gfkzlqgcq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/ggsczxfvi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gwundtuop.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gqwxujrtg.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gworubbtl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gqryufyqd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gfpdgbmdp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gizhjznkc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gmtougapw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gttjpercg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gvqqkgaeu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/ghphcpowe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gqynqijag.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gmpsjkanj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gifnembpr.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gseymecye.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gxpzafmmc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwvxcxgbi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gxzaxnjew.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/glrkeziej.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnjiwdimz.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gakncqmku.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gwupsvntx.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzorsuwze.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gxhfynzqf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glnetydfs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtbtohbdy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gkbirzwkq.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/grjsdouxy.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/ghgkaasbo.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gxhnqiwwc.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gsanvmlzq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gwyvglwwy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gxgesbadt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gerhrxayc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gwcabweld.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gtdxrjhit.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gehbfbwbb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gkrfktpkr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gyzjdlhku.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gwpruseds.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gfdpxlvnc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gkedkjvbq.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/grzjiknvx.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gcaycdzch.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/guwomyofl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/giapemcza.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gfmqplpnx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gnblrrbre.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gbrfkkscp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghelamyxm.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/grtshmtvn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/ggtxddxeh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/godhsmtps.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gskzsjaji.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gfolzgxae.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gphfjkprr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gsmqsxeds.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gtawlgihf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gexusbzbl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gjnjpzdfs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwghtdwze.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gwocodvjg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gsoqagsxw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcvlvwuhg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzdoozacx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gavgtwpgo.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/grceclusj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gwdsbykkj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gxqvtjitw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gmyirzeqs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvlzdlwcg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/glppbnlld.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gzvcsxevx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcexupvsy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gjhjxnsxa.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gqjjczcwv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gqktkvyug.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/grutdzoml.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gfdjvipqq.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gozjduykn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gexepqmly.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/ghoizivaf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/ghoefqyps.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gxtkdopgz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxqhunmyd.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/grzzcivpu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/goxkxulyz.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gnepejynp.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/govfsmgtx.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gbbgefgfp.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/glbitegpn.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gqkqkqqow.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gnjbapyju.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/ghjgeqcsa.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/geoaavrtm.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gxkppsaae.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gapiapmqn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gpkvkcqqs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gpcxghtrd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/guzwzvkll.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gayzuhbjb.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gpxouecyf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gdsguezbc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gjxryqjrn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gurfdrgqr.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gzyzdbvjc.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gfdcytrzj.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gwfryougr.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gmgvjsowe.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gxntsxasw.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gygsvwvac.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gdghnixiv.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gpoxhjtdi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gcazjxvno.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/geahzbbzt.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gybltleev.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gbeiiyegp.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gvzebukwh.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggaxomwze.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gzqkxpyso.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gsngufxns.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gekmmrnuk.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gctkxhprz.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gatgugwkd.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/grwuibnkf.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/giifwcupv.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gehacdckq.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gcijqrjie.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gjdbdhuil.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gnldzbyir.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gidckvoaw.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gtmjaxwhv.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gzeumicns.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gpzlofzuf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/goikxskld.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gpxkypqiz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/glaaijjzv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gdhukaqwk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gxnjofihb.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gdxuaboin.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gxzdllhen.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/grkoiwmvr.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gwgdtlyfg.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gweyaufuw.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/ggivaijmz.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gnpmlandb.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gplechmhx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gkhildaua.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gzsgkcrxk.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/ggeuisrgg.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/givnnhmcw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gitdbmnjx.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gcisohwde.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gjtxaucor.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gphsyxmzq.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gyrhgzrek.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/glruteyre.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gxqsbiawd.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gyluwegnu.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gliptzpdk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gxegrmgql.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/glgxctyxp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gxfxeuznw.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gmsgxjfsa.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwbzpxmsy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gexquitkt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gyiqiagtc.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gczearady.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/ggfbwnxfi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gvepxsmje.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gygmfwfjq.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gstgpbhrt.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/glkxjismq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gqhpwkudl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gmsxsenyk.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gxskzmnrm.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gpdbawhhq.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gqmamvoan.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gjmatlitb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gfgzxoyyw.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gwhgfqash.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbwhagvhu.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gztjjbixj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gmgfjdvjh.sHtML


<!-- 参考信息 -->