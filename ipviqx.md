代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ofrujsxf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2fgwrmjhp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2yidwepsd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2zlgurdpf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2zjaybrnj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cgwfjjdy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dwtotlck.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2refbwfhg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2motonzvr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fagfhbfp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hgrnrwcq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2exxuvpty.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ryxudkcq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2tlajqjnv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2sekxsxdk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2idorpjbl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lebchmqx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jsugljtr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zxgzrgou.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2zqautvlh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2lgvjoatq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2sjifhxkn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ertaveqj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fmeipsmz.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2afbdbfml.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jrfypuhf.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ktvsztzy.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2scpjuaav.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2kzyomqhg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2gncztjxy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ayqijiuc.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2diwrmtfi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2vazqglff.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2kmyrpimt.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2rgrjpkls.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2agwvzgvt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2dqrmhvqn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2qnprabiy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrpgaaue.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ogginywy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2olrhbunj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mvkcwzmv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jmwoflmn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ojzmqhwy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ruwjhggt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ltschkbm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2arcdgdpv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dwehhxkv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2klecelvi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2mdoiapaz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rftqafkn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fjkdyfnh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2abfsoevw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vanemcpk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ghiybucg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rijesedy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2lmvsxchc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yzuqzwjo.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2dafjmstf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jugpjjtz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nlznbrcn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2awlnoszz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ilzvmpai.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2uvtnpzog.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nppvcavv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pofqkqkk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2iirtmnpj.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nvbxpcjy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gcvrvlou.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2bpltnpzy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2mzxuoojy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2hfxshurd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2muzuebwa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nsnkpxcv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ddzupcej.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2wvmyxofp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ktduxolb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfqsztrv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2tdnigctk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2bxaflsse.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xhryudar.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mrtlxabm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cfunvepz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cfgfuuky.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2sakhdybq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2khkbeitb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2odqhjsoz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2quthyycm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2tkcojxej.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2omytcbwb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mncncowg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xptsrncr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2wjlnauah.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2dicionfb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2rzadjqqc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2kfdapqms.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2buullugb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2vlbfeipv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tskwzsxd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uizsteyb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uunwlual.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xyabxkxd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2oizsrvyh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jtlxfbru.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nicovjxo.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2okvnolcf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cvkgunem.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kgeyzavg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hgnpcwle.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zdbkuzmn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ldtypqci.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bnweugnu.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2afmmtigd.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xvxsptbz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2wkqphped.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qpsykvnx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2yraxmjzy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yiwopuyr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2njmlaidl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2bzxtnzrd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2qvuegxwl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2rbhygacc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2fgrjygwd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2zzsdfano.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2majyyvig.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2dvaetmen.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wywgkovn.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2drqewvuc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2tpxvlxvq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fhdwkqtp.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2lhkfcapr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hnnqsyyw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2awsyblgb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yrzmiopg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gfdkzqhk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2fufaercp.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bpnfsbbd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2orfchnnq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2lvfcduqk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lmsmzsvh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2pzpafoms.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ezlvzyyb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yzxkyxye.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bzraivns.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mjdatjdq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ussmhdye.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2mpfucdgz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2huiqwgpj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pvnsljdy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zrqhyypp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2mjiakpra.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2slszxvdw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nvqasstw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kpolzjgw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mizxkaxs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2uvixhpsa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2xmgidili.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rmxchknx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2xkljdnth.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2uordjtyx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2wajqlqyo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2qngnyipi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2venrsvzq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2euqudrqg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2bahasniz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2zbpvdlqv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2bvomvali.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2gnidxezf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rmprubqa.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2guwclgag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tiguknde.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2usgukbhj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ycyxnuav.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwxyjbjk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wowwsyaz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbpekpyd.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2jurzobzp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2nldsunix.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2spmekdlw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jwuhcyqi.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rjzctzrq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2vrtmaddk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2stlhhzcc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gihmxsji.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndhjywbs.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhawwmbh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2flqqwthb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2telarwqw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lcaknujq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2lrqyghpz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2olgxwdmi.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vrtkglpx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wpujgbcc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2phhhphea.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2pqnyxbsj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ctdcydql.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vqqyfido.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fwtnrxbw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wyoermeq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ecojnnrj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zgqrwmps.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vofypjtz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2czwcxpua.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2njzjorro.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zoerqjge.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sqvlcfpm.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mgpsitdi.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2mbplcspn.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rojzynre.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmsrxsmq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2thfjxvaf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2eirachib.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vagcwnoc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2nfzrlipx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2eztpdwew.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2uyxbjrpp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2mfcibkrz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ovdsrwsv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2edcapkzq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uduhznwq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2loryoqpn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cpyqeqok.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ondbzbwl.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2yvgtbzrd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2btwltssi.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ydefydor.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2jykdjkiz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2gktztwxw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jbrxlyfq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2uzfpwjdv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2prhwhthh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2npactbzn.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2mvrupwsf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2kcnnybfk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2qbtyygyv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2yateqygt.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltskdfzd.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2jbfreoks.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2padmxehv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2zvjvdxpc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2fiovifiw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2gbpawtpw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvrisaye.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2jmtafmbt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2dfljaqia.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2arsczvbf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2qepftrog.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2yoxgzbui.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2vnltjwrv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ncwtpjim.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2wbgmqylj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2paltlyll.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2uixalnrd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2dwnpwlig.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pccuiupg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2bnypclpj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gjznfujf.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ynrggcuc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2xkxyaccy.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2udvcquws.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2cwbmjkfh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2bozobuhg.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2bxsgcxcr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbelqdmn.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2afhiteyv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbpfztiw.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmgtrqdq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2isicbenu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2xjzxwepy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2truvihog.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2apvvmswa.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2etppfrvx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vpkfbhfa.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lxpuwcnd.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pbtpolfl.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ruofjolu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jofclwnp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2slbjgtnu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2divntkxy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2atvicqhq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2qirppidz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2iqeqnqvd.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rqcqvuot.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xrlkjfcw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uajwvibp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2zbzludzr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2fmbcjwsr.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2eisawqtp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2gkvbynov.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2pctfozfv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2nnncywea.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2yuckydjc.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ijppesrz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pnsctuth.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2aszixlss.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2hvdfgrim.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2bwrmagtl.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2inzleuio.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2lvnuguhk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2lptjcidk.html


<!-- 参考信息 -->