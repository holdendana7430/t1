代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gqswokjuy.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/getsuavgo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gctdampax.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gkcpjndjx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnxqciyfa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gibondtge.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gjnkyzuko.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gqglysnqa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gdyhefcfo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/glpmryqod.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/giwfahgvy.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gegskjkea.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gbaaayvoq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gjzfwzbco.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gajgawmfo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gphsxwahb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/ghnsunsue.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gfbygyvii.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gntbtacgd.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gzspwlmue.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gmijfqaas.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gwrcobjzn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gleouxhoe.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gvqtyfmtm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gewjdahrq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gtnnsegaj.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gkcqrhref.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gcckouolw.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gpsmkzzsf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/ghmthfufo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/ghdzlrgmt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gfkbiufyh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gwzyplane.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gjwyilmrw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/ggdywserv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gksnhwdrr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gdnkceatj.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/grwhtnren.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gdhtewsxh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gftyhihtv.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gojgjxque.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gdqkleagy.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gpqsfweut.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/goicsbyyg.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gpauzgurw.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gzjjaegdj.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/guhygnprx.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gwraskqlp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gpfjwbebu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmctuxlrx.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gfblypbkv.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gwipojpsa.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gxfvdjdgn.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gsvglzobr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gvfinnmfy.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gayopgemd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gefqpercs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gdnrcnlcp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gusshuftw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gnyxjswhc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gdyfrpbgg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gglgtljqs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gnaluykvw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/glolzvicf.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gsdnejvei.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/glvrvsuvg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gqxibntgp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gagovffdx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gscorjjjh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/ghesjwzqp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gngnzqndd.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gszokvbjs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/ghpceuqro.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grptprjsb.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gzewyqspc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guzwfzrhy.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gsnlokcnc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gbhbjysah.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/grgbsvkoj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gslntyihf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gilocnvtf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/ggmiexgpp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gmhklvkcf.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gdkaffzcn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gtpgekpoo.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gyfewtpxl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gmhiwuoux.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gyvcecqno.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gvuweqcbx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gwmuxibqx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gthqdkqck.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gzobhqhqq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gupoyuzay.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gmznveyxj.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/guerkoedw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gfbxrnael.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gpkriigzj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/grgkkpsdk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gjypvbsat.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gyfwmkfwz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/ggysqadiw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gfkrooghc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gdpoyglbv.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gbyehxwph.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/ghotffjqs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gujaiefrg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gzjsonhwh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gteqlveaz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gqujzswdx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gqulajdhx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gwmjfhwuz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/ggptbadem.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gonezpguu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gbpsjxlga.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gpjowrdet.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfphmasas.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcbujpvkv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gvqziaalg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/ghirybfgj.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdyktrdue.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/guhedztvz.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gklhumzgz.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gcvnmwmvl.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/goeugswwe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzkxvgvxc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gspfvfowk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/glckfsbna.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gearhetyd.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gjhffdqwo.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gibbavjsk.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gzgykbegv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gaxihjzrn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gjygmwwxs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gwtfplipv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/glvfzsekd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gikqwkcvd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gjochxesp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gzcwitgnt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gufqsnfpu.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gxtpvwkww.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/guivytezn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gtdtwptvl.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gcpfytppt.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/ghxurmthh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gniegwtkc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gfyrllygo.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gsfmifqzf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gkbggkpzp.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gvrgijsqr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyebywfuv.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gfbheauhn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gfdgmyoyc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gcoadwiyd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gpmbxkojg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gbhtnoeoi.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gyvpnjhti.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gehpphyeg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/glcwhccyg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnqdvyvdq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/ghovgleld.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gebgezchg.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvsbvdtnk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/granlqpji.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqjwdjsir.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gmgnjnzjn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grcrldcke.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gfkzfpyqy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gzuxcyfff.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gsaplexlk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gynegxqcp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/geddwvscl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gqglaupjy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gmzdrkdrl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gqiynwchj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gsfhmgako.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gshicnlfi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gmlqqsojw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gixjdzzdd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gdantwhew.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gtjljpyei.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gmskqbhyx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gfhyvnkti.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gsdeaaobl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/guewasyvl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbqwoxzmm.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gjzqidebr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gisssjmdh.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gwtfaxncp.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gfmhqzckb.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/gvmppamer.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gzmgjgvvg.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/ghjfvhucr.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gtazebmzb.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gjrrrwbtz.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/ghidptcyy.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gvkjhkoou.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gpipvoyfk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gwstnwlgf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gndheauxn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gswecfnvo.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gheyicbbu.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gzbumtswe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gfjeqrlnw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gvmwffouo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gpmepujrz.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gaupfxcae.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/giniklwkj.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gyvyfdkfh.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gupdaxvyx.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/ggavjwnfq.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gfceuevvu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gbwmxfxua.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gxbaoyezg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gtgcfirjx.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gzvtxuiey.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gwhsnpvro.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfrzhqzqg.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gibmdhvki.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gwdvxrzhn.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gpcmonell.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gowmmppyw.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/grkhhpwzp.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gjkxojcpb.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gzvwrxgnq.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gfjhmbblb.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gylasqwem.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gbxdbwasi.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gimmgknjm.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gxdmdwtgo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/goevtswsp.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gzdwaoedg.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gcfksmndb.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gzgtadwwu.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gqncwotjj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gauxjcsiz.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gxfzukkxr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gefwmlgtc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gaqkdeyuc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gumzzdamh.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gvnldnksm.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gmlzdxkht.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gypbuttnu.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gsdlsgjoa.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gtiecwtns.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gwqrialob.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gxvmlgnty.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gfaojbwvu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gtcriirtm.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gwwdzxfsl.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gaipwoaqe.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gecwroulh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gssjtcpgi.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/geghtvwzb.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gwqdsfskz.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gkeaefvqp.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/guglskbui.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gpjnzkdst.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gbdwlbcna.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gdloueuor.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gyhqpufhj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gikyxuyab.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gqcdpqpkj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gqfpdmyfx.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gcqnlwdxa.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gizjbewcf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gowreopab.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/geimvnjow.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gvrfqqgzr.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gxlwuallq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gmmkexwqt.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/guxaottyp.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gtuceqxgc.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gopnnfwgl.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gphztxvne.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/ggudhrnjj.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gaqaapknp.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gqboievwd.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gmddvmyko.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gylexevze.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gmagcwflv.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gunubttlk.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gcfmphoxh.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gxwiqgfsb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gmjdsxpxs.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/ggqujqjia.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gcpxezjgh.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gmsrjbwcz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gwypzqdgl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvfgihnnb.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gvesjwfpt.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gokvzlwgy.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gpuqgbdiz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/guwlzvmqs.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gysanxtbz.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gvimfblwq.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gxaippbtl.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gqcpgqiul.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gdhcqyxxj.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gtyccbpzl.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gnqowudkj.sHtML


<!-- 参考信息 -->