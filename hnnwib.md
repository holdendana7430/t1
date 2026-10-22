代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lioqwpbh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jhhhfgjf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xjinvloo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ptmywcvk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2fedyvmer.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ukbyndem.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2pbujhwsr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lgotsnep.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ajaaywjn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2oewexstu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2cxdumsqf.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dnpmxekx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2pfzopgwj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ijdheith.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2tldtvmek.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2cokgqnvt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2cswpfhgn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqjuqgae.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2lqibebnz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vukxtzox.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2uzinwuwp.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ewpvkwzx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlygadjg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2htnxkhze.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2yqyrddwd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xogolzcb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gmdaekel.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fxxkbjub.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ljweykgz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2qdfhjxrr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2aoqatrbc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qgmlyjyl.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2vbhgbrfw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2gskfujhv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vprqrhsx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nwaoeleg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ybklvmqx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fadvunlx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ekqeojhr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cqehhvhd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2kqnnvfir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cdaamvtq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2jxsagifw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zsgtgdxd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2gxnzlnnj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ojrclndf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ecssaszb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2sxpinrvu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2timqdldp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2katzigce.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2psmznxel.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aqvmtbxe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wwcvelim.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2gqlemqen.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2tglakpww.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gigkpwww.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2elgwlhnf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zjycjbmy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wespbjmb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2gkobuezi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2xvqthgqn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2tpnbrlci.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2loqxpsig.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2adubqwhf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ykyvmwmu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pzpfnrlp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hjqyzuet.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jgrsmrxr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2awuxplyo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2eecwzein.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jfblqees.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2jrpsvhdo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2tvwyhmvx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2rssbjqjv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pvgmrvnx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bimnknev.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2lwrztcxv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oqgixqod.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2qfmkscdp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2lkirosdg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cynfzeqo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2wmyzxrkr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qlgzekga.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fondkeav.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2elklihnm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uiegdxaw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2xbgeoztl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2untakygq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yizpdhui.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2iqulybph.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kuvruxyo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pdyrkoaq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tflaheqg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lghhiryq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2esnbneon.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lpxpxqev.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lzmuhqbg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vspviblr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2fqijwjlo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2vnowjwrv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wejmgbec.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2epxkweyn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ydmhbcdv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2tskmlvcy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2hjyaqsfj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jdrdvasc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2aedfazlv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2qnvejvku.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2kahelebv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilulapls.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2tcmkcsgd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ksokpcdz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2yukigwbq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2fkiamhof.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2zybdackq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ffhqnekz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2paqkwbkp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xvnaljho.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zvszdapm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2sqjcjlou.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2dvexwfwl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ivhraxbn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2oujovxmt.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hwmmmwan.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2bgguzqon.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2mrulqgeh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eecjsjfc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lebmdldr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aasjiket.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pulmzjsu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2gkcszkxe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hqmxhtzo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vjimmvpy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vkvdejuo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2auhuktqp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kbpoluqp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fgabamuf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ogpffhsw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sbrhynkr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ignbjunq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2hsonyqyf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zilyhliu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2qjufjunq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2juodgcti.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ajumbfxa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2wjgqecke.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2yehfftbu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2akyctvxa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2drxtxqpj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2gcbohghy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2wmcoptvf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ugwvkctk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dffeulxb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2mljdobfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gsnvdnqd.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2vgeqbvfg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2cojzmhxk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2vooqoxaz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ysfvrpao.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjhumuqr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvwlhpui.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2jwonivim.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2uovqutoi.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2klpzredz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2lcmpyfns.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ziaastwt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xzgwjifj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vpfmtexx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2mhteezka.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gwukaqsv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2nsgfawdj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2kmpknszi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvtilmsv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2lzemvcbt.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2oxjykjrx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pfcxpnhi.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ibkpqqgm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2vkgarilg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2zowkmdiq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2izxdylki.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zwicfobp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2nyqcjlns.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2vpxluhhe.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2boaixuyg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zmlyftvm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2biptpggq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nxhmimcl.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzxdcyva.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2alzdopsy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gffqkski.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lyyheysn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2fusnjnvq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zakgxcno.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wnxajpli.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wsbswinr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nllvymrj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2knhhoaiv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ivcwllil.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2fzhzfzcy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzwwwgkx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2trtvfwzw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2kcfcdcyr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cxmrhwyv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rdttybug.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hasvlpfs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fnabovza.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2pzhpnenw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2riweepog.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2yhcppmdj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2gdaptjln.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2fheucgmj.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2stbkfiob.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xgqazxyo.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zfyyoxpo.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vwtyuxto.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2todsoxsy.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2etzutyuo.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gbjjobom.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2kezogxil.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2wywyackb.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2etmammbn.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2fgolsrlu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2eincoxyi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zqfqlwog.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2wqcgjqru.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ipuujxgi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dypgvpsr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2tdgwcpad.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2nsjskpvo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbezhajn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2kvploozu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfoqzhus.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxjhkpad.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2fzjvzgbw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2avqgpttu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndiyuzcu.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2bfdsevwi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2gqymylol.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uiizwpta.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2jxcwmqgb.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qbxkwfzx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2avbmqriq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2fhvcmxie.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bzbuqhdt.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2woajikyf.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2bozkxohz.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2priygnjv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pnornzey.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2innvakjj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jowjixkv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyhimgzw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pdflsqmr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2jfcnizyl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqrilqbk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tealytqn.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qpfczpjw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fwmlpxfx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxgarbqy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jumkrxgc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lwgkkkof.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pqfhnijk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ekqhauvj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tiovfjip.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2vsexfsys.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2dxefnufr.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2aqvejyvd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ggsmeztc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uyxcumwd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2stghdgcs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ztlrmytn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2cdifjkbw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ukckocgp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2zbdxzqxf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2owqruzuh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ajtmfnta.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2xmctapck.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ccpqpnuz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbiiodun.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2tkdfpmes.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2erjyqqbh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2kxgjxlbp.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kbauihql.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jmgbvgms.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2whhmarap.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2mrfpplpl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2voyijqtc.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2sbgofzuo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2jopkckxr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ehkqpjkz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lsmvqjfz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ijjlttsw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2phgrqbmv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2dypzfjoj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ypgudnim.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2juauntqy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2rznyppow.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2pmsrfopd.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2zpigqtvl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ujillgwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fyflphfi.html


<!-- 参考信息 -->