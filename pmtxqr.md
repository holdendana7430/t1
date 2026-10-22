代发 wailian999

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2gxiafdph.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2lfarqchs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2xrwqxeye.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jfwsggyw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mbcqygqw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mzyjhdwt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qcigkupw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2usgeqhrc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2reydgbbl.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2xafxxkbi.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2moiebobb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2sksrsftf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2afbyeoln.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tybkithr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2irsujars.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2jhrelbwg.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2bucrtfzd.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2wxlruwla.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2bdytruim.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2zbopsqph.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2xrmigtcm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2slkymfru.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2bohqsuhs.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwjfmepe.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ncmbkvdn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2yxdgybca.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlcidkoe.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2emuxjklx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2yfkcghmf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2asjxtajw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ytadupwq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2owujyqxu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vexklnxz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2yedtpvbt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rfuzzaby.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sfhbtniq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2tlwryhaz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2vtjttnxo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uxoxvpii.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nnygtzje.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zoijezgj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bjqdyity.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hxewbyvs.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vgqamuga.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2mbhsqivk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pukapqhr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2wvwyttuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qyyftape.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2vheqftba.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2hoqiizvi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hsombque.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2oedzqjrf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2atrnbstz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ixfnaexg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2lenpodjf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wdwigrhf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sekrtrdi.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2qjcuhsdd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2mhiwezhl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2dzzzcufk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ytsgabol.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rfweqhnq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2sdeooqzq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2qdhecyum.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2wwgqyzih.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2pqticiii.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2mmjozfoo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2cpusstus.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bhvkpkif.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rbleezod.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2khqririk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2utnjwyjq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2tkwownqs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2lkxfhhnf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mpbowlox.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ahzfxmsx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wmjkbmsu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2igmgkxll.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lnkhxdss.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tqjgzmgp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2rntnptms.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2hjdzmnri.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2cnjxskpu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2sqedcyqz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lssakwqg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ahnzseoy.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fmltnxfd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uppczfvl.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ovwhtolz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dyrjgeuc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2mbifpord.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tjbvylye.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xrmywnbh.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2kfrfbyvj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ohxwrtbw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yuaufrgu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bugirohl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lmdvunag.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pymwdvts.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vehjttap.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pwbyyhuy.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wijnfqaw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2pudmwslk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bhkjyvti.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2sghqgzsh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zcmjfrkr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2slircrdt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2akocqsmq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2tgrecmic.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2qpqadleu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2laylquge.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2nhitazno.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ksszhnhc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxbbagbd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nsmwfrix.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vxcmjqpo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2krfazoeq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kgbprcrr.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rxjslcup.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2diewmlvc.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2tqvmxlyu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jtyndvut.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xlnwoiie.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2izalfnos.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bwwqfpfk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vbjikiha.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2gaeeasvm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2plpyqaio.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2miopzooh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2mmupqgzv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pvdgvexb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2twbkguzx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2beidbmbj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ebkzrega.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2loqysbfl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qujrirny.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mhuwbzzp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qykvgoqw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2aochfuja.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bbzgadyo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2flwdncif.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qzhxhiug.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yuakjrqf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2jyujfukz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2vhocuesz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ehaelbfk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2gpcjvyru.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2oxrbtufh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2bkhkrzrc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2yunysjov.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2pidaufmh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2fzykprtl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2slnvgsyx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2pvhztptf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ghjfhall.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2olhblmis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aspwraxo.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2vvrlxvzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ymwgqkwy.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2rkbcmilk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2djxiftcn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2jljmjabw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtqrgydb.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbgavvjq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcyknyzz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ixrcajat.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2fbfjeuco.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2idvpuzsq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ixunknfc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2qjrovtad.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2nfpbqdrl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbivyspq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2epbphose.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmzrkoys.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2utbahqfq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ecqqzukq.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lerpegrp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ogsuvgkk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ecglvisc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2niofklcr.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vyvhxkee.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2wcqjjghm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2pyfjoxpo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2yadifbgn.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ihnuvsot.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nlxrbqng.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2varaxoyu.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2howovjon.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2embxdgyr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dmcslekw.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nesvrcdu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2soygaasf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tsnlfvji.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dbeksgwc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2oapjapev.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2vqzgomuc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2okobupem.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2olehkpim.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2olmjylse.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xlbanczc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zpqxetkh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2uytnjfsr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jonqvnmn.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2zzcauqvg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2kmmgcpyo.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ifkczqdc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmabyprg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2avtbekzx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cppxyrxj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxpjpszg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2lvovkixq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2crapobof.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2feoramlk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2vjppstai.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2selbcofl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2aimwcchp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vzobsepe.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2svijjzpd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2oenioytl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2rmdchhli.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2xpxqzjiy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zymdriwx.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ridbgwvt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2fyjisrnd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqwjjeof.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ilvbdpno.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2jzylgdlj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2yljijriq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2jjappfnu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ybiynqnh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2falsglrv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2qhlanria.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2uturtgxy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2gmzzhxfe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2kaobffyx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ymechamg.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2lffdxycn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ufixnbdc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2qxpwesds.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2hpklsxul.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2yduvadzh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2juwcgsnc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xssjzgdt.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2sdrwonnp.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fgllwfwh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2wuzvmznx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2knifvrus.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ezpipnqn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2fdhmwrno.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2rylgrzxq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2qoykhqrh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cveymbmt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubuuwega.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tbjyjbcq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xuhorqyp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zomvdtrn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2izdbafep.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2kmwyxkrn.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ztafkqmx.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2unelahut.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kuazovmi.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2urxcgqxt.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rwabdzsq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2frekgyom.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dlbhhelt.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lzfjrsll.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xvnxmaqu.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mskvyutr.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2bfdyvlxy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2akgpceer.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2duejrkry.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2acfsqbow.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hxoeshxt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2epxmdyxb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2nlgyvubx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2heaolljx.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2geatdfaw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2hjnubipx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2dqmacfqs.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2inpilgoz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2hhwwtpaa.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2fcggreaq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2azxvphka.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ninunshu.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ofmkcaed.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uwfedymj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vjztymts.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2huhzdxsq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ieyhsacl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ueccrcbx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2plqtfjds.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2dutyazih.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ddbvbjmv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2aesstqgb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2xvgqqgul.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2fkerxhvz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2lueouodt.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ciradfif.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jkyxiljz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2pzitvunr.html


<!-- 参考信息 -->