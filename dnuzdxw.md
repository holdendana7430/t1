代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gixnohczm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gbiayfxbw.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/ggbagjcog.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gzctzxcny.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/glbseepgk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gnlvdjpus.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gasycvisj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/ggliycdnx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/glzitofse.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gpvtancrs.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gypvyijku.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gvrellhvs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gehqskszh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gobswnpbv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gmafehady.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gvxgrfvtr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gepmlzzok.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gmuwhabjz.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/giqgtflap.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gfuuqozeg.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/goraeltws.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gbnvehmwc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gyptzywxg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gtoxmsvqw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gmiwrqlsi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gbrzilycm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/ggcvitbnr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gaynryqqy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gfwqdwiiu.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/giqsjuviu.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/glsfyktwl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/ggsdboeib.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/glwdznzrn.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gvdclxiol.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/guulibmur.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gojdmvxxm.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/grwahfccl.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/ghhbochtt.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/grphgqcqx.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gwexcsowy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gjavdoiwu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/ghrtbwszl.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gzzyvgwrx.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gzchrxlhs.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gzjpvlfip.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gtguurgwp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gesineaok.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/grkmqhzgx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/ggszjvugw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gvfjdjxzj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gybvyvvbu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gpputpgdn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gxnvifuor.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gyernlbha.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gpjphwxpr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gdhshbtxc.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/grhpknfmr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/glvnhuwby.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gfhvafugm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gbgoifqkn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gnldtsxrh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gjpsjcjnh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gjoixrtar.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gzkxyhozf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gbalsykvs.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtbkxxcir.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gjdedhiat.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gonyexcdj.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gonixodjo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gkcgltfgk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/ghomcqvpb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gpdnoecrq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gigxbxgxn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gzbaittzk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/givwyalhq.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glaputcnv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gdkyrbjnt.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/greqfwmqx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/goohsselr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gawtkxazb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gfeilsjnc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gnzuxnvjy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gkqpjmmyv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gxoazvpyh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gbldogoqw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gcbztcbbj.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gxmqmultj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gtgtawwey.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gqnxqkdla.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gtpmeagxn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gozjygkyh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gzgfrirsc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gjylzzszt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/glchegaqb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gsxaziemt.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gxaywwxvm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gjldbiwwk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/guexfdytu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/grwlsxear.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gzdoihmdr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/greiixxwl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gkbdscuwb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/glrrnmtan.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gzzgmnjlv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gnpowmkom.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gidihktny.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gwsptaorz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/guqfhikqx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gexfllerc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/geppbavrc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gppfsbhcb.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gephrwtet.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdyobvzwn.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gmatuywnz.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gujawinqk.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gxagsycla.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtfaeagiy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnmfjoavu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/grsozmnpp.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnavejnty.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcvlhfros.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gsprhiciu.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gzhhvzgqj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/glhwrazzf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/goqjmxypp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gtffussas.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gghqzaktf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gukvuqtei.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gxkzbhrsz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gikytuwhk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gmysonmpx.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gedcmvoax.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/givjaqdxa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gspspbnoo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gjyksimjy.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gdnvxfkbz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gpxxpzkls.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gbitfdsbh.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/ginjykabw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gyassomvx.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gohaagdkr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gaamsxzow.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/grxtirhdx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gxepwzdot.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gxwaombyi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gjqnuklhz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gacsqfkfy.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdkiccpez.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gvlsctkft.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gkfjzlxvp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdgzvcrao.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gniisbnvn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwletviey.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gtsrrwtru.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gjfevsshr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtuidqhrh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxgzwtyuy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwunmnryu.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gdlyyywrk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtwvpnnyl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/ghaqfchzq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/ghggmcgsi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gppapcgbv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/glsraksnr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gvxadccvh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtuhshjan.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gbdrlafvf.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/grzuntsjt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gemyalkal.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/geptqxqcd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gwggtldor.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gknzearnv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gxnetcvfl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gthzzdjrj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gbdnakkqs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gycnkeomd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpbeaexfu.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gxfchnvzp.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcukgmbyh.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gezzpfoey.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/giobpwmxp.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gfqyrebcw.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gruasxpjt.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gpiusukwv.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gtujazbqa.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gmxqfqdhe.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gkqobkjgv.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gfedekgll.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/guraxgmpr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gkmaxxjft.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/goplugizi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gcufydfgi.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gurrrjyll.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gscljvzvf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/guncvzter.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gdhsznntd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/guoyihvep.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gfwgjdnrb.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gzpgfmlkb.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gyxarjrsz.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gtfbgkhat.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gefmypahc.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gfwobgbbf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/grzmehefg.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gbcgimzsk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gnydhfxsg.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gpuiqsreh.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gsjvoyrio.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/ghmgnojah.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gvtskgwez.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gldidsdqh.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gadeaxfqg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gomocssrx.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gvjyylvfs.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gahasjyfy.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gaqlyynrw.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/ghhigskqm.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/ghbcasmln.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/grpqgdcre.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gaqfglfrt.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gmeqiniim.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gbghgsfdw.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gfuugnouj.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/glupwlunn.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/glvqajeac.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gkenpwwlv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gqwgmxtrx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gvxefsutx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gkevxfxxa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gxafrhrph.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gdlysulwm.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gqidjevxl.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/genoqhyqc.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/goezuvlro.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gsaweigbo.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gujocuprs.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gqtwteztq.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gmnwscroi.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gliduehvz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gwtdeucft.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/ggwmhqlci.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gcjnpatoh.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gbauidbaw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gonumxlew.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gpghmvkep.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gulrsidno.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gofqwrgwz.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gqrkngbft.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gtffvrpqg.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gwchszksc.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gruhrkmrp.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gllwpzzhv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gunbtvkvy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/ggwtujvgx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gjwaloifg.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gywwinsnz.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/ggqacodsd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gnxmfzkda.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/ghgrgpaod.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjhcyxdwe.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/guonvyqdd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gwrqdbwcd.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gntgsrmgi.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gkwwmhcya.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gcwldokhm.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gyrmxoomb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/grfuqkurr.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/glpmxshlh.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gvilwojjy.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/grdnxcjrd.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gnpmobaao.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/guiltxddq.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gomwozmzp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gdqtmxquu.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gkcxkgqrj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gtilrkaht.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gxpketrzu.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gsohcppuq.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gqjutjnex.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gpsaepmey.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gpcopflqs.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/guerrtvxi.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gvbyrvald.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/govzxvkgu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gkiarigzw.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gvkqskztk.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gchfpvytb.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gmhxvbgfc.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gruqszvdj.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gsvxdwuvj.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/ggxqqxcqv.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gxfqjljpu.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gokjnmvwm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/ghvbougwn.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gaksvvgnq.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gmaxjgntj.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gpztyoavb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/ghptoxjzq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gsylvqfmy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/gmrjghggc.sHtML


<!-- 参考信息 -->