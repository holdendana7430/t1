代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzepudifp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gekumkcrk.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/ghmbfgjzm.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/ghhcmalkx.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/glrenieha.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gdjwuckus.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gzlfirzkl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gwdnyqadf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gazpcpvla.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/glfhyaeji.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gilqtxpul.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gfkikxuar.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gksrkqrad.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gmdfanghq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gszndcvbx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gyrnhdapd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gmjjjikjq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gngjopzzf.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gxnvwzxvg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gexrsaula.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gmxelqzvf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/ggucwcoda.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gnheqjcju.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gjlitlxsk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gwbqlpoig.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gpxrglwqi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gxmttrxxs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/glpnwnmow.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/grxsajeym.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gmkejeiob.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/grazutiea.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gkdjsmuno.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gujepwinq.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gwflixmjz.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gprobotgf.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gmrsbgnfy.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gbxbiauxm.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gxjhpkljx.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gzlvxxtml.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gglywwqrm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/grsvymcvz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gprcmqomn.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gqwfyrczi.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gbktsgznc.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gcmucdarr.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/giwzzhyjq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gkbxkamas.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/guryjnqlr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gattejgvw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gvmhpgrsn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/glgsiouil.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gbujezumm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gayaekqbt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gbicidqab.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/ghdhqsixi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/geyeoqgou.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/gcuvqqmuv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gxdbaonxp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gvppqjbxf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/grnezatlq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gehbakhmp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gmeguvhyg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gkqppdpdz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gphwzewhq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gqbrhzoqm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gzvhnkndj.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gpvtlyskb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdmsmxkth.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gcjysartf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/giuzxupfx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gdfhyyqcf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/ginbntkwl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/ggenntpct.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/guxntnvxc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gnapysxyc.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvoxtcwew.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gwkmrjhhb.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gvmtgrizl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/ghbrcjolw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/glrbshmkj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gagywzoim.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gdhdodclf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gjymwhdkg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gnbgaschh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/ggpyhoidk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/glmuankgh.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gnnbxzqlx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gylmuglfk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gqbjotnga.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gofoxssgi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gwnbrieyy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gawrfvjuz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gkpjnrstn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gumucvesw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gtfbnkzkl.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gelkfteyi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gczwngebx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/ghjgtwwho.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gliqqqgnt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gwjxllsnc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gwkremanv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gnrkvfsku.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gjjemfcxb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/glpsodmrg.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gkvyyzjzi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gwxuxuqyp.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gauvcoqtc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfserzpsm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxcoweivj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/goofukvku.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/grwkeywba.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gsjalliub.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gwyvbvhwd.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gwuieyizr.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqdhinuvp.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gldqyjlat.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvgodbdam.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gnjzvsmif.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gjbdompqb.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcuniwcha.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdxakqllh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/greveclsi.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gekuxryjt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gzpjfaepj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gkydfsmso.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gjkjavuvj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gnhymgnqp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gwugvkote.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gbsmbjvut.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gqbvzsphf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/geewqhbdg.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gqbsbvsfr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/ganvpdnqy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gqurtfcuu.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gajsocfax.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gijdelcvc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gmipauxdd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gykpvfxeu.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gbnaeazrw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gtpzornvk.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gtweewhfh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdvcmdypy.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gdtqugcni.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gwymihoea.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gtpqzcaqf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gpvpuztev.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gkhsauipr.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gluuoijay.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gkcfzshud.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gotcucsbq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gswerdhob.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gxridtgfw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gocpydxsm.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqicojrfc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gavuhwhjs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvdsosbcg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghhrzzbyc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxbzaomnq.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/glrzllixg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkkvgayhd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gynohtgsg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gbkbqcpwb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfznsvrdu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/glywgaowq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/ghwakhgml.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gpksfkixw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gvxiuvvku.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gpzumyrvr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gajykulmx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gfxeallby.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gzrskafxz.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gpwzzwjcp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gcjwpkxpn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gcratkmyq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gyzqcvxzu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gjumyuzfx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjkvfcpwf.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gajbswypz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjkixjywg.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gtjzlccrs.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gzqzrikaw.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gidkqgpdd.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gthvotkgk.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/ghtexxkfi.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/glsmnuvao.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gaopgxjkx.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gmujlwefl.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gccxaqqmt.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gvvikprsv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gfqdgajik.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gssxxpqho.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gpfyxubgl.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gmhpbfcwn.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gnjctsyfw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gokjwydqn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gfquantri.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/greiauvhi.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gtqbqusdy.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gdxxwtcmz.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gjgqqabtv.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gfbwbezjl.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gbxuamjme.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/glsibxdbq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gdwsvdimg.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/ghdyjtqqa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gcmzpcxnt.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/glpxtirts.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gynfyglck.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/goliziztq.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbopseosu.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnjlynoam.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gndtxdiwi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gbmomomnv.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gpicasdth.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gnqvkypel.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gefnfygcn.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gshjzbyrv.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gymcfliqf.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gkuucrhkk.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/galijrkfl.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gqyrqeumx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gqyskqgpw.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gekfxbzxg.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gwblxsfbc.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/goeagadth.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gwsqrkmbd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gqfzuyvpp.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gxavvjsfy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gvoeskinw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmmyfwmlh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gunthphek.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/ghysmptvb.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gfcjuybve.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gpeotzceb.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/ghbznqxnq.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gwrkrzosv.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gpmjssbzd.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gbwfcotek.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/ghqdospzj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/guwiqcxoo.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gsczzdvjp.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/ganvwaudn.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gazglqxmp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/ginwuewyd.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/ggyjanwgx.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsvgzwusd.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gskhwcboc.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gcsziyznq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gtjqonmda.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gqwblawig.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gycaowoaf.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/grimwotlz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gizoewnki.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gfwailgkc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gsfxqhxgq.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gmuzhvggy.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/guinrpwmb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gwqdrbfrp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gsrxmdczh.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gucsxidnk.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gaqdmngdj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gyzcyibgl.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gjnpqgxeg.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gkpdmfkln.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gkehpuebe.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/grxjphijg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/ggmscxicb.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gixpmgmnq.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gcbnqzzxt.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/ghsvzowgt.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gghangdfj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gkyikqunl.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/ghtzdiake.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/glisalofj.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/goxxdrxof.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/giplgxzcy.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gyvbukmct.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gybudjylt.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/ggdkmcabl.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gitccxago.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/ggcynjnsy.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gcbtjfsxk.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/ghugfuaxm.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gijurkxgm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gxmmiumsn.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gjwsvtbdo.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gvnucvlvx.sHtML

[G13] 判断对象类型
来源：http://www.share.fehbvm.com/Article/details/gnjaopdei.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gyipxdcxi.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gxfqfkvxy.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/ggmlbnlyu.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gohfrgrpj.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gtbtzcehq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gvzwktymd.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/ghkmeurgq.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gwiahqadv.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gywfnrjwo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gbaflnnpv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gemjvsjps.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gbktuxhuo.sHtML


<!-- 参考信息 -->