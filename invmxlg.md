代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gqezpnpra.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gxqgwfrnm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gfcwaosnb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gweyynypq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gwygejkzr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gbvspdehl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gddxiedwi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gvwkapkth.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gaspwgxpe.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gvrxgjlzb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gedzduirq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gekdtkjbq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/glhaqmhzh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gjklpdozv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gcrjetbzm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjfynomjb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gadddwnwp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gabkrdiix.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gsazbzywc.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/geeadodgg.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gigzfljgo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gfoxyrjss.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/goppiyjth.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gslcglvjm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gvztddueq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gdnjxhwge.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/glmfwduhq.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gzfsybaeq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gxeqzkccj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gkadbitrg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gjveybbyc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gzmfqeila.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzvzjbxng.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gewutjwrf.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gdjhslmpr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/giiabpeyd.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gbkrasbsp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/ggmhrstil.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gmronophy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/geeadipzq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gcbkcizfh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gctawqxoq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gcjzzmard.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gbltumwai.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gomtdlkba.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gcvdusuaj.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gjvghimor.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gtebiqmth.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gsaeewmff.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gyxzoufjs.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gbaroduju.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gubyalorx.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gtwdipwkc.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gafkaxdym.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gnzllimnr.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gakzhsdfp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gluydgkav.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gjbamlrqx.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gcqfsoxvy.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/glesizhut.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/glmzekzhi.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/giwxiqwsk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwgbrpoyf.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gdkpcizcu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gzjqyroxx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gcoexbypc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gcyihpuff.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/ggtrpevpl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gswqsmkow.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/grtnnvrvp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gbnequpou.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gmhddzzdg.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gqebrvqbh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gusjqnzvc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gdzqtsmkv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/glmxnhovd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gvjtdaclv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gxedsuwbt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gcdmbrbke.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gvlvjwcow.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gmprfzlwu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvlwxyiis.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gwqigjqej.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmoarkwcw.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gvbkyvmvv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gvltroehj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gvyvrilbd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gtidriaeq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/ghyxilphu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gpfzjcetx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gjjmqvdrs.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqdesytdb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gkzkpffmj.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gkgnmakuy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gvjuymdlg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gjgxdggjm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gsbovldqn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glkhjivax.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gloqtmtbv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gyidirbqo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gvuehtayh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gkcynszxk.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/ggcrzcpki.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gvxbmrtsl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gjvlgdpht.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gvuqpbdtx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/ggpdsvebt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/guihucovq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gszyhsptz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gyxfatocc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gwwyrjlxv.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/giqgzbhhc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gcdoxdxdu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/giufjkois.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gsdiaiafe.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gnjeidpay.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gmiuhtfxw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gchtrjuho.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gaietauim.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gshkajqrf.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gjgymsayb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gdkgsgyzf.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gzkvjlikh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpbcdybde.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/ggagcdklz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gucmjgjdo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/grnusevhu.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/grxxtbuxu.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbryyontp.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gsxiqswvz.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grlagtsra.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gcefkswti.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gzhdbhaps.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdgxvmben.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gnnopwfln.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsmrafifb.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqzvchosp.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gzqusnofk.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gsqlqfjvf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/guqsjlnpq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gtqehpqwl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gtmksyajo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/genkrbouk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/goukrhdyw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/guhiuhtck.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gdogkfwnf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gkjivxbcd.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gszakdfis.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gcatjakaz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gqoxtnxtx.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gjrzpckls.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gyrfzodav.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gekylmnth.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gmszyzojn.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gtdzwohfh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gekhbqneh.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gmxrfbtrq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxnqajzrj.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/grocsmkxd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gmdcsirid.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gfbuldqgf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gzeiytevk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gkdgeahec.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gscnyxrsc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gyfqrczvh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gqzblhciw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxainutje.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/ggjegndxn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glmbrsjgh.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gzwupbaes.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gnspvswjp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwhjcaldq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnjyfprva.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gjuenjjkv.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gejtclppr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqzthdsgb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/ggvckmlah.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gmxbkrdxm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gmeelmhor.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gtcjunnum.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gbzojsmqw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbeeggcju.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/geoilkdaw.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gdlohtwxv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gkmhjtijk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gitpdoidx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gbgkzwdzn.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gzdzwuzhb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gtdvhkotj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gyioxgkqd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gykjmzqiq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gfuymjbpg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkdremwgh.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gzdkcbrvn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdxcknxyo.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gjqilcqph.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gdgkyawzw.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gikwguprs.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gihpwabgr.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gcyfoyvvt.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gmiezlaih.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gxeajwlri.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gdnfaxljk.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gyuofkexs.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gtcpxfjbu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gqrdlsfsx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gwbnywoly.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gydobhpxq.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gqwbwrwfd.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gsuafmbvw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/grhnilcmm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gjyscixxh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gekvojoro.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/guxrlrbis.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gytezaxvi.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gokniomcr.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gmfvbimwe.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gszkhetpa.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gbaiteomg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/grgednjdn.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gpqsngrdm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gclfnvfti.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gtrxiupkb.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gpzttpgwz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gigcxlqmp.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gvepeyhwx.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gdatkksco.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gamblbdpd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gszcrrfgv.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gwygswosq.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gsfhhbuto.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gxxyjptkg.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gpyndorso.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gspkywrob.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gnpxdnsxa.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gftxbxcha.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gdyhdvfjr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gacnurfmg.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/goitksvkj.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gzgbisktq.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/ggqzvvrdd.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gheqkjzxb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gsonmgxvs.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gixetfmkn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gqtivjqjn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjkjgmsfw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gfzcjvnjr.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gnsjfhgtr.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gexbqncmq.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gvhxayaqr.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gzuemuqfu.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gnwyzepzi.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gyuhfdheu.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/guzewnqjp.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gofykubau.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/glenvzkzr.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/ghxhttaza.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gfbbvqfyh.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gefvorbbh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gtyqihprv.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/glksdvtwm.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gaetkjbsg.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gyaptfzrf.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gljqrbjjq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gcfenjple.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gvkncnolb.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gxqyugkqi.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gadpwrolf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gesqpmsvd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gwjofaewz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gnmflflfe.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/glhhynfsh.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gftwqufov.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gvqdaqfqd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gehiawuay.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gryawbiiz.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gvkfsvdmb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gfgvreknq.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gvxobodfw.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gdxrsdiiz.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/grwhdnwda.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gkjobsghv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gxawywyyv.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gmjqquebp.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gicgwlhsf.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gaxwbnuqw.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gzvffakhs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gysxnhoax.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gslibdvry.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvulznwkz.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gyotpaycn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gmiwemsss.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gaibzvhnn.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gkzywhrsr.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gxaghfkoq.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/grtboltdx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gnxmsjalb.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gsbtblcaa.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gkbaxkvuu.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gswsnnnlw.sHtML


<!-- 参考信息 -->