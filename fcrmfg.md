代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fwvyetmd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hfsnmlso.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3blobonna.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xcsehkbd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3kjkoqlfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jikqlbop.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3likpcqhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3udaldwum.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3yecrrxpl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3zjlfgouj.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gjnflvga.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3bltgogve.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zkazbxlc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ffmxfwla.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3divvpofh.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wiosaeyq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3piuevsry.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3pgbzlvbk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3iqtlhofj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3psqpkoiw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3alshejil.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ynhxewem.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vcsgeadc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wpfixwot.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3dvytjjyw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ijuzqdro.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3lzqbbqgm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3qisfexvk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pdqeobli.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3doedyndf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ttlfwnpd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3hdqnefin.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3dtllooqi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3orstalxz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qzyqpmnd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3polcddgf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wnuitiep.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3foampynk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wygzutlb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ospnicut.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3zlkywfmi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qylglozh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3kmroihub.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3lfzopesl.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mbmundnc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3sccyvkde.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uzvxwwmj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3refsvscz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lojsssnh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xfgxflfx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3tvphznvd.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kkouvlie.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iyrahfyw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qsbfxzup.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nasbldgr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ncgwedhp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wwwbpxia.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sqvojulm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vjhvusxi.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zficldhk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lctlthrq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rekhkurw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3wcezxcvd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3psrabhzs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3dqjcmszp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fkhiojlt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xgmtbieq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ruquhxmy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3peyopupj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3oehagpdt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3wbllnzdg.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3rgfkydlo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3hawjfpak.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjavfqqu.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tswwlyrv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3toznndfs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kkgaeyfg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3fmobclic.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ngnhuemq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3uuqjynkq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3mphmsebv.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3frqbapsw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wxlksmdp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ozzvfyfl.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3bkhypjyw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cdhzyipx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3lynmjzbe.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kqcqlhfs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ckpghjky.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3uckdyfex.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qpbnfggm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iizsycdc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dbjoglqr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uffvkuxb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3dzneoerd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sgpqxbtf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cdbtayoa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dihwrnzl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3udpwisyw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ovcwuniv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3emduirbi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fyluxxvi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wzebaumn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3weobajsm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3lwlkmcot.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3olqxngqu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3kqtsvled.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ctbkujze.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3oipmlwpq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3kiirekgm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3tupnsctw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3iljxysyq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ieqzyzcp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3avwfoumg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3jmqasvwe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zchfwudo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhdkvrjx.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3bvaarsbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpkgftez.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3lmutchgw.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3jsdyzukz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcubzcmv.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddpiapjc.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3vkgpisyt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gasybqhj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3pkuiuube.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3niwfggov.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3egljrqpv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3usbfehkd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3toouqrgo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mvhwnwqb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3sbfgqdzf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3fmukmfnr.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjstubwg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3fepuugdg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hssrdaym.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tahlkwmf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3zinyzcwf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hkfkecjg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mnhflhwb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bozbhmgu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ufduaofw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3eldrlzuf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3fprawpqt.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rhrkanvo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bhptsmel.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3avhmgofo.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gdljzomv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xybwnivo.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxapcxht.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifbieest.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3epefmycj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jckhfiak.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3evdowxpg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3cvbeqatd.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3vtxpggox.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3uxhysrpe.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3afkmritz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tshgdpze.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tifbpkat.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qolaidts.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3knflsdtx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3sgrpbfbo.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3wnfejwla.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3vsctappb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3uqzoavaf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jkhlkjix.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iknzhsph.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vugllbqo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gmhyiwzq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3jwbfcncl.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3rprlopef.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3oeqkzfbc.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3soqnmxgk.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ysifvwfz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vvojfnio.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wjxaojdo.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cuutfqmf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pbcucbsv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3lvphcfmy.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3hgpyovxg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3koxvvenj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3fbxblmlk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3jonrhgyn.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mmtxiprx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxakiwys.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3vjdvumze.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3aubrwuin.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3iecmsjfy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ubfiqjsk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ycshohkx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3wxhnzyrt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3tvyennkj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3sztnaosk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ktusgydc.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3tklwerxb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3kmjhvzro.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3znwlufvf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3vuppbdyk.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3trlpmwcp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3cchgxkvo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ovurealc.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3evkqazkf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3urfayxew.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pvkgekeq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3vmvgvrww.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ogkmlgem.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xstebjyx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3yhzdkbjq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3abbraefd.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3kdmklnqu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xoqrkgdj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ruyvsmsv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkjlbndb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ujkxeims.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nynymjum.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3rgjrlknj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdqgxokf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zieaoziv.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zzpwbuzw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkxamajb.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dxtnlvij.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ancflzxm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqnuwigp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vgnurcty.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qodhnsjj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ygstxtai.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3xvvwvjxi.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3yrhclnab.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3indvxtrx.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yjbzuxna.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lnrthfjd.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ewebtzlo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3amymtcrn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3dttfyxlq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3xmiezyqg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3nfyolkfh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3jvzdgplz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3gtphushn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3stppsgva.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3wmmfesmw.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3kjamtfqm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3psepdwtg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3nxorlyog.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3vojyirvr.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3evtbsusr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3yqgpqfjq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3gzdjprfm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3hdmevlqh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3erxetcre.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3mqlkppiq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3qfbhmjkx.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ptazzrlj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mscbwhco.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3zogfdmso.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3owmbkrqz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3vjrmtasb.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hhrfaldj.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ehhyrtkg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3pfsvglga.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3pqybwrnh.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3jpbnkoks.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3zhvasdxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3upxaymst.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3gekbzjld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlmeclro.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3refmpuqc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3seznahrk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3vnckgusb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3cmouqqfs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3osbdybag.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3nrulbywx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3trackblz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3eyaytrmr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3qthbsjzt.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3lekpgupt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3kicuntax.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wymfvhsw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wizfzdtv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3iainjdmg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tfjcohqp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ijwzwpkb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3vwnktqay.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cgezouqx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3mgbqbywj.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3rzpzqede.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3perengwn.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3basieogt.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3btexzobg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iqbimpad.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3wypydjfq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3hxwphcig.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3brezcpxs.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3imctbgms.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wpvbvzur.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ldxehrij.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3dzycbisa.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfzdycjl.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmabsbqy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3zryhhmdf.html


<!-- 参考信息 -->