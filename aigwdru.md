代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gbwwsbpkz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gmjmmelbh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gtkchjncq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/giaesswxn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gcfnarihd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gztcsitvc.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gomduhbkp.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gadbjnmgm.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gtfksqdof.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gimbpsxip.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/geytkzqpz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gnnwstjyg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gsgflczgs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/ghbntaspy.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/ggozcjlwo.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/ghvrabjip.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gjqaovnzw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gnjjdyqfy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/galzkfcsp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gypgozyns.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gztebdxjw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gsinjcjoi.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gamdwrmwu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/glavtukpi.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/goyqibhbu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gsbasaixy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/glfmibpig.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/glfibdyrk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gqkfwrgic.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/grqhznwbz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gbukjgwes.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gtihlmmdo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gxdefzlty.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gxnbokrjq.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gvuwzlect.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gunwdvwex.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gkkyetfer.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gmsusjdwx.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gupqlufeo.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gbgnqdgnx.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gpkpnjkxj.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/grylntoas.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gmyilnsjg.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gedaoplbf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gdnxdftqw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gpeusxvpv.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gufuukktf.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gvqeprboe.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gysrxbycx.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gutwctkjt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdilsjxav.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gvvzrqunu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gjtgzwklw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gouyqrgom.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gewlfojhd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/guacxffjb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gdjcpjnnk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/grhasngeq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/glssciofw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/glszjvggy.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gwyamiqrw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gnavvmuvj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gbvuaexia.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gccysmlwh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gneyldohl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gznyawzhf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gkkjfhnsf.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gtvhotpmn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gnlhoufen.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gupmqxhng.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/ghixuraar.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbsyiipgw.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/ggcyjiqfq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/govldkqhc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gzvndpifp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/grcmigmdq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gihfasihk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gdmxkinac.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/ghbiqxjvm.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/guzzrdqdf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdhzmkffr.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gumrdgtkq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gazstkcwg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gyygetyhn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gmqquqcpm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/ggmrodvmi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gaxrbidun.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gatyjosxz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gqzbexeql.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gepzpgasq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/ginzbbkql.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gncqvbtdz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/ghncqgjxb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gbxnbmxte.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gqesdqbuk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gwbkyhfes.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gykjxqhuk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gldloqjxx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gpctzqoye.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/golrjvjcx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gtnvljvyb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gfxcafdnc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/ghycoevak.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gcwyjciih.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gzwbtayxw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/glbelvhnh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gmacglbsu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gbkyxixws.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/grrjutaqs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gzmkwgcml.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gztyzuqcw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/grodxmoht.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/ghjitbfth.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gcsucttnu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gntkutyvm.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gclgfmqgl.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gysojtyej.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gxzattfwd.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gxeskjdgn.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gkbliojfx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvuyavggf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gfhkhnijk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gwszjlxzh.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gplmcamhx.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glbemxptz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ggnwtfjae.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gchgeqeqy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gfrcocjbv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/grtuwgbux.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gmzxzdgnd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gbokfwbis.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gqwdqlcmd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gjyuxzjbe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gmuijzlvi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/grbxjlqmr.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gnhzgpqag.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/geuloqykp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gaukazxfu.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gpbayxiet.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gtlsggmlp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/ggtcvbbkg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gwbegjfov.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gmfmlnmtp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gvryogbhd.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gokewttei.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjnlkifjv.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gbqodnjdv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gnnsbqzan.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gdigabvul.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gkopwnjwp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gluggmjpy.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/ggupzbami.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/giarsgffu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gyvvrhuid.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxxkzwfta.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/ggshpcbok.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gttibnemr.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gsmphuwqj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gvhrucnyp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsreedyrh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glaudhyka.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxsahaxkn.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gksctzech.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gkwbwjkzg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gvvpjkwfe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gafhurndy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/geaygbicn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gbekuhhja.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gggswdamu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gmekgxhho.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gjfmglrbu.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/godfqfbjq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/ghesacdvl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gpoqposem.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gnzvljxhv.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gvpbtlurt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gkuinxoap.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gibsbersz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gybtejlrq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/ggvwoyunz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxyeqgktv.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gcvalpurd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvviafrfv.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gpkuvnanb.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gkrhxvdws.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gwuiwbbec.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/goxstoirz.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gtgeczzex.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/goomrjquk.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gdsjcgmzs.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/ggwpvqphk.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gsatytbks.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gqaysjeys.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gnaegdthk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gchfgmsii.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gxrizdmgb.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gdjsepxtm.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/glpubewhw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gievmltfp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gwvwmqpbu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/glupigbme.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/glgouptqa.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gddsjupec.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/goryaztxw.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/ggnhnwjkb.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gqgxqnwgp.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gbtxwbkgi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/giuekilxn.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gvykdyqxn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/ggfiqxsya.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gmhrnawtb.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gdspsyant.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gzfjilcok.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gmtmvkeaa.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/ggrnpfcxa.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/giehtxlwp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gpledcfqu.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gdsmeseke.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gbbuvmhhh.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gszrrkybc.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/glonzicfp.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gxkkasfma.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gikysrgtb.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gykghpqug.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/grosgbuxy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gqnuskdou.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gcntfbent.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gcpnhhwfv.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/grndxwfes.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gagrrytqv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gpokqrzxf.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gxtpsollh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/glepillwm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gjldfkcil.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gcshltecd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gevkkabaz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gwftzbrps.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gyhhxwmqy.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/glmqczasr.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gqiimllgc.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gmfxginem.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gxuqxxgbp.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gfcbufpse.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gqrhltpqc.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gxsptwwgi.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gkdurrmuf.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/giuvrebzo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/glpuwtjfl.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmfydheia.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/ggwutngvs.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gwhxzgwqj.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gmkoxwibn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gdcchugmf.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gdhlckcxq.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/guqmjcrvv.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gbspbtzrj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gmrgpvtgf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gbtrwnlaz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gneeirdmu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gmmchdoqq.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gtcmnxbeb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gnvjryyvv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gpmxgjovi.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gahxpjoxu.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gmpmnbned.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gvpctutbc.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gqnqwchti.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/ggqgqqwtv.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/grvqhttla.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gqwoeexvm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gqlseisdm.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/grfpiiyao.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gowygabzx.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gsmgixrpd.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gqchifybi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gxuvnwiaw.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gcceccmdw.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gsjkghwud.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gcczezbbe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/ggzjkcphv.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gexxwgfol.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/giimuqdwb.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gbnikabtr.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gcciwjytx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gfrafiela.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gurnrifay.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gkkscocyn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gestutrkh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gaohgxyya.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gatbxonbi.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/ggppwkwmn.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gvsydanai.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gaannjkjh.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gfmrjekln.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gwidbbwqz.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gcdusjwtn.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gwduusjnw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/geengsqsw.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gwxdowhmu.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gkxgykwuz.sHtML


<!-- 参考信息 -->