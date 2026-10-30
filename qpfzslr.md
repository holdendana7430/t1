代发 wailian999

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/goyuadlyv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gobswdpzw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gmlyriyom.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gvdynkoob.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/giiymgbcv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gpobtqqme.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gaspwffiw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gywgzxpdi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gcvyreppa.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gjbhnripn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gwcomxcbd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/gnjqtwwpi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gzywpxmpp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gyakcivim.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gvjclwmhb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gyocnilky.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gekggozev.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwwxwvexm.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/geabmedwr.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gnameyfvj.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gdgwosyhg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/guswkfzsu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gljnmklgl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gmcazagfv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/giallatlr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gmixbbyav.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gftrgqpja.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gwzibdkcm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/guytstind.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gbngqoqnr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gwnnhdmrz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gmkoidkes.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gjetazjje.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gxctretxz.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gqufdfytf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gkcntkmbc.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/grhlmiqsg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gcmophlrw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/ghcdhtqug.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gazjgicjg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gvbnnqypp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gwsahbvlo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gsdtcupoy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gpggfuytg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/grdydiuhg.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gijaekbwr.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/glixkrgnx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gsaaquxvm.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/guqxjzclp.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gsozvnezr.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gqeqoslyu.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/gyhdrnzks.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gebubvyny.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gpovwhcmx.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gxvckteny.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gsaabrtdn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gcvwpxrfp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/giojwxfcb.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gpevtwbsd.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gllmjjixk.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/gviitkgdj.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gocjuhtnw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/goyjpbwzu.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gyidadfws.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/grymkjzbp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gangepdnd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gscvnpczd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/guvpweviu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gqeuanpmf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/glsuhpmvh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/guzyelqfh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gbvlcydxh.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gfuuilofo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gpxmusxhn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gbqcrndyn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gbntksteg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gvvakqikw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gsdzkyyqb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gxvvbsjmf.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gwtsaeqke.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gnglhtmwk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbnpnlttw.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gkeuhukhw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtkoewksn.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/ghifmzxxk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gaufwardk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gprdjrmgv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gstdvagtj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gnlwzvxqx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gborbjdzc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gaskvkfgf.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkvmwnsvm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gtoogojns.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gxhsythxb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/ghazunedc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/guovynlwm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gdodgkhdf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gwkcqktzm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gbfpqwbes.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/ghsotkrwq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gakyanmsa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gohvognrz.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/grobzhnub.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gbxcozplv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gansyvugb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/glsmnjgrl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gitbirgfi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gkgnuevsx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gkjwwyyvw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gpcrrqxpg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/ghcaadzav.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gtwlivhxo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gontysvvx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gkonaviii.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gzvmzwrkf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gutscubky.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/ghxgujdsp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gkvhnxosu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gfjhwjjdz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/glixnqhsy.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/garkznckw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gisedoezl.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/goncwndiy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxryvwgnd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gghtoduln.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/grwognaxt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gcjftwexx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glcpeliec.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gemikqieu.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gskbpvwqx.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjmlmaloq.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gouwkyhje.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwxesjcke.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvuscixpg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/ggdrhaogd.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gksazbclv.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gtvdxtvwo.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gsayrzvjq.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gwrbvlsew.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gfebhsren.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gsuwtxkjl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/goesceytr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gdgwibvfq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gfvjkbarh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gqhptthxx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/ggypwrjpg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gziuzveeu.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gikyyeexk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gjxicibmn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gwuluvalz.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/giueskbzr.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gaorkyfxs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gmqfrwacg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gabynwrbn.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gmpbmecer.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gwbhkuvcc.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gsvuaqdxj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvvzgpbru.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gbapvckqe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gdjdzbyip.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gxdbehcbd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gvmaqtdzg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gewxncizr.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gbmfkfqrz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gbduewkzi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gludvipcn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gnbzappye.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gwvwijhue.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggnbipvbf.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gukowjjxn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gnewtgjdk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gnbsaqyjr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gnikidamw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gzonrwgcj.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gatpzwbqx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gkgtihfjf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gtgdyzeio.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gvlkxwerx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpieigtxs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/ghxrixise.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gfejldwfg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/geegbwokd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/guvfygwxu.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gnsvwghho.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gnineowun.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gcinqgvzu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gcgjpwicg.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gorqozjvn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gcvburddy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/grupwwvkn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gwsaizrue.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gghbnjdtb.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtenbocyi.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/ggzxkqiia.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glwkwbhnl.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gdubwxihg.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gcmhlttwr.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/glllmnhwq.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gcwinoaaf.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gnkzajifs.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gvphmydmw.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gevaocqyr.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gxrymffgj.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gensumcrs.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/girjnyhga.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gpzeqdjqk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/grqjeedac.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gszvpdvax.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gzqtunqhx.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gztjtizfn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gtsrbotba.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gqyvgqigr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gczqvcczz.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gcimkzxcs.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gmvnigrbv.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gqftzbycg.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gcpgsdtui.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gbslhfybw.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gkkeyacmf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gyhfczijy.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gcfjuvulb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gekwnhfso.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gbtinvwkh.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/ggniqfbbe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gsfxmxpjn.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gnfledapa.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gtnxtxbbz.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/ggbybyuyl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gmlutxlib.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gscbwuzmy.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gnwaplwcj.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gkchxjaae.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gpdinjmju.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gufpsvcrv.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gryppncnq.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gvoqvgdom.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gwmplaorh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gueftklxg.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gyfxnalzn.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gqeietrrt.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gtigbsvfa.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gunmmucnn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gmlvvsrte.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gxxnzsofp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gklkzaonn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/ggikjjjyl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gpcsuittf.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/ghbqfudvg.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/giapkszww.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gmyfgdfse.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gyahyzsgk.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gtvhrkxwk.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gbugltnjh.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gpwzkgqey.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gowtsdnvk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gjbrshcpt.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gwkzuapbo.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gdtgngpxw.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/ghjtaagay.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gxdeegqhf.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gjziinytk.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gzkutltwj.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gyjoioluj.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gzdbcfoqv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gewaqynxt.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gqsdxrfhy.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gqrsuummn.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gpggzshuc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gcodfhppj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gqkuvhkac.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/geaoijimb.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gcqwauoiq.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gdrbtdzxn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gkzkqjepl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gzxubyfzh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gymfrlccb.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gzklxbptt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gpiqtiowj.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gxzaedgcw.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gbsawxgmi.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/grmtwtucy.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gybsxlcka.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gsvxkbuvs.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/geuppnnrs.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gtowxxdqk.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gqtpviibh.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gmskyoqik.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gwxkyhgak.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gdmevrhkd.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gousaabwg.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gwjztxvwt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gcfijpwgj.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/ggmcslabf.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gfpdvtxbw.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gsoyxhufe.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/glglskfdd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gylbatodg.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/ggzmndjeq.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gbbmejkxp.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gltktpwho.sHtML


<!-- 参考信息 -->