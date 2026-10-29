代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gupaqylrl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gotwtxxhd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gzctcrrfw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gosvopjau.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/glfahayic.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gtbdydxzw.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gkpfqduca.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/guwdngiwh.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gemozemwk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gipjupoaf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gzxugkqbw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/giimiqxhw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gvifequkp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gdhjtxxzn.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gryacwflh.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gdxtxfopf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/gurxghqxe.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gjvccpzdf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gnhkecpjc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gaetiypxk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gvqhitqhr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/ghneklsds.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/glxclsika.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gnqwhgvmb.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gxoxcwuck.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/ganbzvuhq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gultnhikd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gtlveoxit.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gytxyasca.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/ggppkytqf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/ghuikrkvv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gwkxeyhqm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gblurvkif.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gftytuink.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gfvgkkqqd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gmnjvamqo.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gqtmqfqec.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/goimnnjlp.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gddaczhqa.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gpsebbxtn.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gsiherxog.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gwvnftjux.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/grcydfony.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gjphqomyk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/galhvmeee.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/giriljibq.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gkxuhpjai.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gfvlsaewg.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gqawitejt.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/grsyrnvzs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gvchwnvky.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/grtworoty.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gifqocagt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/glqekztnl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gnhqccfdg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gcctbhnbj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gxwcdunxj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gxyowmrra.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gisosdohw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gtbjdrmkt.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gkjhxyifm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/grvsqnoyv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gothcbczc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gjhmsvido.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gpryrxxra.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gfffifnav.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gigxipfss.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gqffeanmp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gjjqhhqaz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggjltbyzg.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gnscqrcvc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gdywwoiez.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gauapethj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/givzrqiqp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gqeqlqkhe.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gorsysczh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gubjznuhp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/grmbfgykj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/ghdopnuoz.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbihxlgsn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gmfcwhfas.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/ghddzavup.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/ggeaiwels.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gkfsiggna.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/galxqdclj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gfxdzilaj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gbfqgtoek.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gewizwwmh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gkwwjjfkw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gehtsekep.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gwuighkjq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gjexvqabt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gnmuliorh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/ghsxciwrq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gurwoorpa.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gritywrua.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gvxpmjese.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gzpirkftw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gzserjnef.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/goccihzhl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/grgxuetpk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gkxtetcrd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/grrlnnwoy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gsglmeoco.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/giwodginm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/gylayrsob.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gfdkpxytw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/grlcrdeml.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gglzippfk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gdryubkjb.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gbqfxgxjd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkkfmwyjz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gblnexfno.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gmczwocyy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/ggaxnkbop.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnhqmpbbe.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghuhidfcj.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gfbdkbumb.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/goqewpznq.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gxjokamcj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnesamqvq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcvuemvlj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gleyimdxh.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ggpmicujn.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfrtkjjcw.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gbpxfadvh.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gjgsdpktz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gpxnxwjtu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/ghmeynpru.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gsezriqtd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gfrvdbjud.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gkokobuht.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/ghxlgkssv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gsmejfrpk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gmmycvtzu.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gatypwato.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gmdqzkgju.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gwtnnxvvf.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gszplymrf.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gwmnigink.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gnnryvlmq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gmcjuwjsh.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gxaokbyvi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gpsleoajj.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gqrlyxxbz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqlruvrgu.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gookfvmup.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gwrfsnnmp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/ggcubdagx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gyrvxzdty.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gczvmpmfx.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqisolgsb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gazaobxzw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gouyjqpvj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gtddktvka.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gyjkbphus.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/guwjktyav.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gllrhtjuy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gcazjchkp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gbyujdopy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gpcgcgbdi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmyvholtm.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gsothuqhx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/geezvurfk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/ggkqgxzpg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/giucghlfc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gjfbkdlcv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gnjdszdjp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gybmjbuqi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gwgdqjbud.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gkqfgmbij.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gsoibelsd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gljoiqcuf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gjhjvrdaj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gmvorinmu.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gdkmbwxev.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gtvzuhqsc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gdopujfrr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gvspyloxq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gaaigtcry.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gabslmnwb.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gycoxcsge.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gldztefvg.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gszzqkoxu.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gurfbkdmr.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/ghfatbaip.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/glgmhvwhv.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gmgolprwf.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gpwarjzwy.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/ggfjrwgpx.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/ghlchffjo.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gvyzjjkzl.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gwdzdtzlz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gevhfzhvr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gvrgmlpwf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gxkbagbui.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gwqujmddl.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gnnjoaaij.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gncggbfiz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gwfwsothk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gtyuyqrgn.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/glimeikli.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gcuuydhvm.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gveaedfup.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gqekzqbid.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gkrzdnowj.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/grcnfhhxh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gsvdddive.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gqgjdqrts.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gedjryjck.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gfgbmpujn.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gcubwuydi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gyrbcfbjt.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gpvjfcpme.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gcjnifsle.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gtdimajqe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gdopudqxh.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gdguumjnu.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gkqairwos.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gohqfolxt.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/ggmmtficy.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gsidojsqr.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gjzzoretc.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gxykjcmgh.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gkrnbqjkn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/grxhhoosm.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gtqqzfkhi.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gwalamlzc.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gbbebvgqw.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gljfcdgwf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gekbzbdgw.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gclosposk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gphgpgpfj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gmgwzbnfu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gmmmvufvc.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gdtxhxufb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gnrbmmhbt.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gdtlbhuam.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gyxpvtgqm.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gyzcvgora.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/ggbrememq.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gdrckynfc.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gadxuzzte.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gzisjwqbs.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gjoxansdm.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gzznrrxxw.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gyflwhezc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gpuphpbvn.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/golanoife.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gxqokyscz.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gnkhvsfxp.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gfehodcrw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/ghrmrctnf.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gfapbgcyl.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gjqekseub.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gnlrjhnae.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gxjefmcqe.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gmjztmiiv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/giheiwgpk.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gyoltsuxz.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gqmulumdq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/ggoegyfdm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gkftnqdot.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gmdukfdbz.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gtuhxjebl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gjgihgnrc.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gkwtfsgpr.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gviurhqih.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gdjnkhxez.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/goexvguvu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gcjsvyexj.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gztrahabh.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gfpvzdfyh.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gjakqzula.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gjsmmghgi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gbrxqfbxx.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gyrxtzypt.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/grpxcyhcp.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcwtwevaj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/grooaosgw.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gsxjqaebk.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/grqcdegmo.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gplviewoj.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gdmvuxncu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpiwjkdoe.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gulvyrfdo.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/grnlhnupy.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gnkliecmo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/grxlzcyto.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gwjezqcmr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/ggojslalm.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/ggfzjrowi.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gmafdjdit.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gfvbvidzr.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gicvvaoyt.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/ggowwgjez.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gbgnnliiw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gygdbuhhj.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gurjcropa.sHtML

C#:   u is User
来源：http://baike.fehbvm.com/Article/details/gbbizunwy.sHtML


<!-- 参考信息 -->