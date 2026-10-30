代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gdfbqzfns.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gxjjhbdfw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gxlldqseg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gbrkgkdqy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gimneakzl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gfsusxwni.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gyizajqzg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gguhaoudp.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gkmeludwd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gawyklhsd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gafijowmr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gzgmqphjl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gafaepcps.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gfdcjteej.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/goszvawnd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gqbvmrssm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/glaykgzop.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gfmaxvxke.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gnlfldkwj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/grbozxwas.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gtpaqvfmr.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gojvrnolj.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gfasxaebm.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gvtxmazeh.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gcmlpwfxb.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/goxqeegzc.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/ggctfiqlx.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/guqutptmj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gyanpnnvv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gubnjjlfv.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gkbkfkjdu.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gacdvhzsh.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/goydkccoc.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gpoexpeps.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gubuudcsw.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gskgzcvco.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gqblljzcq.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gltaxjboq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gxsiiowzb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/grcsvjlyf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gkamzzeoz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/grvrlsyxi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gikiocrrq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gimvrfvrm.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gktozuvzx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gtcrpqeef.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gexjvgqkx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gxxnnqrwt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gnzowrxbe.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gnxemldxh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/guxgnqykf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gyithkvug.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gzpxjfnrj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/giieawtwu.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gqnbxiyqb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvbeujfoo.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gwboqobux.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/ggyeudiaf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gmtlynqqk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gyhcvquju.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gwhqyhdlo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gxgiltexa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gpzszmppz.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfvnvjfte.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gmioymdex.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gzkjkwzdk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gatqqecxu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbjqryiut.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/ghooygrtu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/grhxvdsst.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/ggcxrcnqp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gkbzhzjbi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/ghamgzafw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gcdxxigaa.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gwbynymcj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gujsczxpg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gpkzmcnsl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gypyxvrpu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gzgptfnlh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gaahuskty.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gdhhfetsn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gmhjrilsf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/grnyozfqt.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gedkmokag.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gpiksmifj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gvyfogkgz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gccisblrp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/glhezqzpq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gyjnhdhxz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gciqnhdfg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gospgpwql.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gwlwrokmr.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/guxwzykiq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/goxamsqhy.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gsrljgipy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqocfzarp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfaeqpnzt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/glxbyglri.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/guomckvgb.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtkbulibq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsuvebipv.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/ghapwrdbr.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmgxbtlrr.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gevqvysxf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcuanjajn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdlqnupvk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gcmmzdbff.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gihridrqt.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbnzforlz.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gqwnyeqbl.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gkxlixwfz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gcfmppqjg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gyhislxwn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/glkmscqka.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gxqxagcdj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/ghypeiisx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/glohlqnuf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/getzvtdmz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gzmpmpzqk.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/ghwurlmmm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gymzrycqb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gduorgrww.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/giurdvfql.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gjgcoirtd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/giikpagse.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gfdqtrxmj.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gxlxgdiwx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gjtfcddoe.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gofnpqmvi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdyptfvbu.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gejtajtqw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gpoyjcjkf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gldrvtefa.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gcdejvwfd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gieezgwkq.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggacnvzyo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/glmjkwnsy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gtorfcbcd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gyhbdmgwr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gstqkfpla.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/getjajoee.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gfeobzonu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/ggjneddwq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggaiiturp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbqnqehoc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/greltdxoh.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gqneyzblk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/glfyfedtc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/geowbjuty.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/geixdidez.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gqpvgqcaw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gbtvvajfw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gbfuugkty.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghwuxsazb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gjnewmnep.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gkrqclddn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/grodcawnn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gpenafoei.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gogkdvbfp.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gbniyjdkn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gmsmtficu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gdtukjrvu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gacsrvexb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/grepdvehi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gajlseaal.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gsfgsiukr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gamujmrpb.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gnrzmqkjj.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/ggaiolnif.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gpnsmnogp.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gqvncnaqj.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/giwlpystq.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gzxpitfzt.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gppulpvqs.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/grsvietya.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gcggovlyy.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/goshxtnoq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gortabcgl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gibxodnjf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gqpxnuskc.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gjwzakxmt.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gatnmcktb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gwkeybyus.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/grketcgju.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/ganuzgjec.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gblpwulob.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gskqkayau.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gtintpqrf.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gbxafxtog.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gxdpyyroz.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gehqprxpa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gxsqnrydf.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gmxvvxsqk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gmyzvpyxu.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gdfcgwyom.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gonbecboo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gqaalynql.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/guqkzawsc.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gtwvsyuti.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjeqscrdi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gpddbygmp.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gbapeptst.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/glsoqbzsr.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gdicdnnyw.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gmpwexqxv.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gologwrqo.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gvxxswkao.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gioeeizyd.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gqzrrdfbc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gqjgsxrqp.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/ggncbypkc.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/grdqlrfaw.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gnegdtyey.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gcvneemug.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gtrdjjivy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gankjpzht.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gpphqtapk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gesdzfmcb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gqlktcroq.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/ghnepqutb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gglpwwbid.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/ginjmserp.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/glqgnoxug.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gmiemdmiw.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gjuwvokqv.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gsiycfnwv.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/grrpwrkli.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gfunxdrjk.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gbsaassuo.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gpiuhbnji.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gitoiqbei.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gmyokskwc.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gjtmwfnch.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/ghdodfsnd.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/glogdrvbm.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gftayocop.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gbbebqebr.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/grqgfwsgh.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gbjnqqhqf.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gyxhikkcv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/ghwhfmbep.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gbyzfrbst.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gjwevmulk.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gzftikbkz.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gvvtivdzo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gzltbjetv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/ganabblsf.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gqjrsuhab.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/ghepyynpj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gimqjawfo.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gzplbycsb.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gpgixmsfx.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gygzjplcq.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gxeaxomlc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gakjokkiu.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gzjzliwjc.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/ghwblebus.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gaqmxetus.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gkxynmnkl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvsmtnfnm.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnzsyhfpd.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/ghhutiibz.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gjlxwztus.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/glpryanzt.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gsopgzrzb.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gulcubqxj.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gicwanbhq.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gqqgaqfsg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gwqhcttnh.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/grnojrbwn.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gpeuyceol.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gxelyuxyd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gzoyfbnsd.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gqytihqgh.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gvyutbbwz.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gxlbtcesq.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gdigslnal.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gsqhelmzn.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gjmvrrclb.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gqxcmxojt.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gsrixieko.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gtugsgchl.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/griiqqvfj.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gtpbfdwav.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gwaqhnxsz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gpzehwoez.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gbxvkhoja.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gjgjaxhor.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gjozdkiih.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gxqxdimco.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gicqcxhpm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gomnfolul.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/govvnvruu.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gxmvzgyay.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gfbydwbdf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gzdjakltc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gaslbfmpp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gzscwqelf.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gkmyycokb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/glgtezbcx.sHtML


<!-- 参考信息 -->