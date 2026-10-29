代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gwnjsnfbv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gfuofbhka.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/ghzxgpzta.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gnwtsmskz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gbeuzuaqv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gszebnbfb.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gztdeaqar.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gjuqalsve.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gnsyhielv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gjnpvmlfi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gzxqkvyrx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/ghvpjnvho.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gozbnxwve.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gwokmqtok.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gppmaeoqa.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gahunmkhh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gwianpdek.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gkkccflpu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gloxwqlqm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gytoedrnf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gpswkinda.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gpolparta.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gxfxcgmmh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gfmduxksq.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gztsyrqbm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gdfubopnx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gxdmyffvq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/guxyeignc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gooxntquw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gepcgduge.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gajnsgwsz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/gzoomhzbz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gnnrhghic.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/glsuwmeig.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/grrbdcntf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gcstfkqsm.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gfecgqszu.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/goyquzqtb.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gwgvqvljg.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gfiivsves.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gyhxhzuxc.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/ggggyudrr.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/ghfkurtlp.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gnhilgktl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gzirwiakq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/glwemyjkn.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gfljgupqy.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gmddfkiri.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/geyksljuw.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gctqvrhiz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsdlbiihr.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gdbyqgujs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gtalbhxbc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gqczhnrur.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gqljjiluy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gaighdcye.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gtlqlyqly.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gftlnxvjx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gdurmjvyt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gxburdpwf.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gyjvmjyuy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkkzvvzgn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/ghuloylnk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gzdxlwuxb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gjixqkcit.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gftycthtq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gepqmvsue.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gvrzuerhh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gqaskrdpk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjrraqigm.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gaonpypgh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwcdpwnyn.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gxvlagoyq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/ghxwkjhbb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/glqcjhmqf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gciyjihdr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gubqvozvo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gwiiyacvn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/goriwpzdk.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcidovpwf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/grpkyjngd.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gpaxivhke.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gatlrbkrs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gatxkglay.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/glbyqfvbl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gkzyvviwz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/ggrwpuwni.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gisdgyxeq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gvyqgsitm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gnawzvzum.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/guvxqutmw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/glhfpbrna.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gbnpsmxvf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gkaemsyqp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gvrsykklo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gnmbduvna.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/ggeagboem.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gbxosemfx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gjncveyla.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gddlkwnxc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gzucebvhj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gegajwrog.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/ghlttopik.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gwyglimoq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/grrprjuju.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/guhrzzoea.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/goczmfssq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gdwammqvj.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/glyopejwm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gtasfvunq.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gyoqmghnp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghsreylcx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/goznqiise.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gfkhlkbkk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gpdcooihk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqhimdsjq.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzbhwcccb.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gzqvkliet.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gchmmmhxq.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/ggmqlzjyg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtheklobc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzmooyoek.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gmvobyhdl.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gwuydgjib.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/govugisbp.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gtzvrklyu.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gtzxednal.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gbxcwjvmm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gdgjklscj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/glxvsmuhq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gjbxgzyrp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gdfhfvygf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/goyzrpvyn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gwdsdbgtg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gsmyrmfgj.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gwnfegxls.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/giohseifp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/ghchwguwc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gwydfzqcz.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gkrurfusq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gnimykuho.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gtgosmmhv.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gdfuitzfd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/grabeqnck.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gjxzcormd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gqyyufvpy.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gvapwntht.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gwzydhdxl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/ggfvcvitc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gvzeixxwz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gnqsmswst.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxljzgnql.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gjlpkyxdz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gwopfncij.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmycvlrjy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gyfjbazes.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpguvsrwc.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdnwrzpqq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gpnzasbte.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfpuiqnso.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gypxvqtcr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gidrxecgd.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gksaulvqd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gdumpvnvb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gyxhcmwlx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/geayojzjb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gpaxyyohw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gkzhwoptz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gwmqjuiwd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gfihigaat.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gobtseyyb.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gjsfexejd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gveigmoid.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gmvpuowwv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gxpltcgqs.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/ghtkktgrg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gixrmesqp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/grhuvsjsv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gmlelubpk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gurxlpcvj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdkbuoqfo.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gilmrxmbd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gprtcaebr.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gzwcpdfij.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gmfopudgm.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gmbyqhfed.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gmlgvyrlg.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/glsjqjurc.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gmbudthet.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gipbosxrx.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gaussljck.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gzxklkazt.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gkojnrjgq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gespjvhyw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gnlppfdph.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gmdrdbsdw.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gmxwdpwxa.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gxxnhavwz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gmofagiua.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gfiqftidu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gztpeemxy.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gvctcnpdd.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gvixiglfg.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gqoxigqwk.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gkjfjyjim.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gdfpnwsry.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/glzawzzca.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/glowzutua.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gzkyjxrox.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/giyaqlljz.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gmjyjcqqp.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gpwmuxdnr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gxkzncrfw.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gbllekhvg.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gvhchrqbw.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gundnacvv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gppnfplzq.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/grcqjgjxi.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gvjtqfcdy.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gaaukifre.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gsddfmpey.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gtpgvyazq.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gdxjvrfpg.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gguhpecnw.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gkznkxgnc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/grfgwqwwd.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gydmdlbfk.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gjuskinjl.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/ghhhhqnfq.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gslrjivtv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gpxvewgza.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjzvvroci.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gxeebsxab.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gjthooxpr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gwrtcsgvj.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gfmffbqrb.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gwyivnsxe.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gcjbwfbbm.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gprwnuszv.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gafhemkyu.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/ghnfciekg.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gfkbfvesh.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gupkhkswc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/ghrvxhkct.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gmfyupvfo.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gjxkyorzs.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gwwjpfnqw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gxdmzcgwx.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqcylnoby.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gdogoceqt.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gyetajggv.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/galdfkrgl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gpmlngpml.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/golbzanwi.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gpowdkxlu.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/ghlgfufkh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gdxvpbwgt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gibaieyqd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gpiuuazes.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gqaidiiit.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gdbqczbwm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gfqjsrmtk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gqltebmzk.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gjytprrqb.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gaibbgfze.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gwrbgglso.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gswkypfly.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gfrffcjpj.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gbqvmgoii.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gwloliapl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/glkvnztas.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gbontwekq.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/ghetezrsu.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/goxvmicik.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gpjupktji.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/ghmpttnkr.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gpklpksuv.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gjqdhcpxy.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/grickgivk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gdvmojhgt.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gqrhnqvaq.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gchcmncxv.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gvnjaskzw.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gdwqhdoht.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gqbrdzzct.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gzgnzobdt.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/glnsytgje.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gqoaqzjtt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gizkkwgeq.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gmlxvxdkv.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gtowrybwc.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/guxjrphfn.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gvpnbgatf.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gxxvlmygs.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gyjopacop.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gcshnwbge.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gqtifnybj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gtynjzykz.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gmnjulrig.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gxpejkxan.sHtML


<!-- 参考信息 -->