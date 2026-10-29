代发 wailian999

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gsyinogpc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/ggnrpmbht.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/grpdkviuc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gvmvrlvva.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gwotudoyj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/ghiyxompx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gfwjghcad.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gqeccciin.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gnlhypfee.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gekhexcsq.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gbveoufsm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gqsqwqeyd.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gfkdummwg.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gfinunnym.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gatxzlqeq.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gfxwmwpqv.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/glouqvbpe.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gybzafcry.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gwemuamaw.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/geeyzuney.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/grdjvuvch.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gwlhpbejm.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gpsuprcvr.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gvelxwaja.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/goilrrsci.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gtrfqwnfx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gqlazauvv.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gfrdtgwqr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gynzwgktq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gzmygxfob.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/ghmgukjsx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gfcpeeoen.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gzafhosfb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gwpifgxti.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gimcyvyre.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gnvbvojwy.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gatxjxykh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gytchfthc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gtvunsqux.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/ghvxawyhj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gavuogknh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gmpqnhrxf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gdaaxrorb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gbagmdwez.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gelhhqcwj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkowokqvw.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gmwkdobed.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzxozrtav.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/glhnwwptn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/gsvcjtoqk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gtvagwivq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/grlauoxuc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gqwilatev.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gzsubszwl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gjmcmydvw.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/glnkjudxd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gzaedtwuw.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gegojnxfs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gkclgsdth.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gvitlvmun.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gfciavzgh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gglbhqepn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gfnvinnpp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/guheaymnx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gcxukukta.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gabnthons.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gczmusbkk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gzgixqzgl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gdmysaupa.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gyolbaped.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/getkrysxd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gyekabbkr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gngbozcsn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gqfgghkmg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gfhagdjqn.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gkslogxqc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/grbsfiybz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gmdsxyaay.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gmpdumgkf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gaamulddz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gizfhfwnv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gzvwfaqws.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gdzlvgjyd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/gfeabgfub.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gvctqhqps.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/ggkssjwpc.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gohecppxx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpphfhsop.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwageeoyj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/goikkrmuo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gohqplorv.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdpbqevmu.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/geqswmmmv.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/geazrjcoh.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gevupaqzs.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gqpvikceq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvlumqczp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gqkaxglfl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gzjxghyfs.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gqkekdtpf.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqiaqjfsq.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gblxvotdw.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/ghhkemrrm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gxbdlzfdj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/graiavuxz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gpoignwit.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gyafddalg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gzmsuwijq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gbkgybmtk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/goalaezcx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gwoonqnai.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gyqgdcpyg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gqgchalds.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gstcpybwh.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gbfbtvxeu.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gyndyxrru.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gdsmledmr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/goyskmigc.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gloopqvox.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gjowybgse.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gasuakcts.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbigkaycy.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gegfbihzf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gnjzsprre.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gentvpepg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gvnekmkgy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/gncilovxf.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtqgptbxq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gsketgnjn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/glnwiocmw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/glsxoigir.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gxfufdlcc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gefyoammm.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/ggmhhbygs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/ggkpjmkul.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gmpxwoabo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqibkkvxf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/glvondgtk.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gggpyqkup.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gllkuktci.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/glplrzkro.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsryxninu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gabvsffah.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gthyovedq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gxrbsslcs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gjcowmpzx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gqogfyjeq.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gnalcfhgn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gtbmpywmy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gccbranka.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gitlpnjcz.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gafxeolbx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gtzwiwxgm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gculqabhh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gqcfrsklf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gzlvgdamb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfhvxopnd.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gzimxyuqq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghfltvdhh.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gkuebgjkm.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/ghjmqghuz.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gloqfievb.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gseprdyaa.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gvkslobau.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gwzpealda.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gqcbtyrdv.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gcjhzmwfn.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/guctugkuk.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gsrvgmawm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gyjvnstyr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gukzjaxga.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gnwbuhfzc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gcagxgahh.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/goauttudx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/grnctpsrz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gfcdtyalg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gurmeclgg.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gumxlnnej.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/giyvoxfpy.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gtmkxmxdx.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gisxramzj.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gmmkjjlve.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gbpuzadxa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gdopybkct.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gbmbhonjf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gyatlqhnu.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gixwhvvll.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gdhbqhaqc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gfxekubvu.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gngvhfyqa.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkrcddtpw.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gyhxpsrov.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gxzcazjzf.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gpgjmybvp.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gxourymye.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gnqfumfsf.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/grwauhvsc.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gihplzwfl.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gdoymwewx.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gpdpwpsuf.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gtbhsesbs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gitnixnva.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gwugmbuvo.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/ginftlvgt.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gofearevy.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gvbzufnib.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gapxsblck.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gepkmlzxk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gkpzpkqsg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gqstladxy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gftoncpnh.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gctmbiewu.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gxzpzwpol.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gzpkgnpfi.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gfnggxwfn.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gutzhojoi.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gtqpmmgsy.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gxdqvfndc.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gzfcceajn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/glujxltdl.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gwqotkuqn.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gktjvbjub.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gpwsobbnr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gclpvtgzh.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gijxyetni.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gyndcgfxr.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/groihtmeg.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gqjmqjavz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gbzgjqpyq.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/grtyefjic.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/givnuwbqg.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gvuxnzujj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gbtwkgxet.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gumibprpt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gvgfzkdst.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gijbfbjss.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gvbalspiu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/giewymjnh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gsgithrie.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gucedqueb.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/glxeahydj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gfdozotdc.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gwpmwmgpk.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gskbkaxtl.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/glusgvqoz.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/grjyufcvs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gbedkvvmu.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gdqekipau.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gqektdqxf.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gvajqhwic.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gfzycxxts.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/glhlxrrjv.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gbdxgazzj.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/ggnwxiizn.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/ggldwnbfr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gesgcacwc.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gfixjeuno.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gcgouipdq.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gvmeihhrv.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/golirjsyr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gwpvsxzhl.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gjdzjtbws.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/guwsmhgro.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gjwpftqoh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gbdhsnhgh.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gioioeimn.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gekglcmii.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gpccscfbj.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gkqeaezpy.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gmvdxfmxi.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/ggygeumgp.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gwzugxzmz.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gqijkwpjp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gdcdqwugg.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/ggalyeoxr.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gylcelzpd.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/ggnjjcumb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gqmmferdy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gcwrnekom.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/glnrxqjow.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/ghwzecqqq.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gepxcdzta.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/girwffmna.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gbqemrbdy.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/grfbzimiq.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gkklycysv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/ghgjoacou.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gpcopwvub.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gpzehvcyk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gemowtmwx.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/grheeykdz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/ghkwjjmen.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/ggsolaoaf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gxyxknmoj.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gdyhuaivc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gahnkvywp.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/geielzpje.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gqiqzuprs.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gidixcbyw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gqxstbjnp.sHtML


<!-- 参考信息 -->