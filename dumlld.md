代发 wailian999

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rwqslzon.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3hvdtxxmj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nzkuuyco.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3jzapeubi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pqwwfmlo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sxbmcefk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3unmbyklq.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cxqnlebx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3krlpctnk.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3tzosrxkp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3okbuqtug.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxukdaos.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vikqcbni.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3bqoueeut.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3rjeanbon.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ccfhflun.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ajycydea.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3igqlwjmj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3sefydygb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3wgwuaage.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3htrkqqdo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3doblaonv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nrtzbust.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3zwxvqsrg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3moebmbye.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ixlrhdpg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3dzlmwznb.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3jbfmpyvz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3stcgrwvm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3tqvbbzci.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jfncdolg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3uohqxbwm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3vpettnyt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3nqswbbkq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3mmdwrgav.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3meadqrxq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3xrjskkim.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3pkirhjef.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vloneehg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qrpbunry.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hrdtawqt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ygvcmbhv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3jfrqgxqe.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aigjclfg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hwoxzfaz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3zkirqcpz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zfisuhrh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fdzcntiy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vvqoowlx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kegzkolb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zqtsxifq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ocnbojwt.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uulelkaw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sklyfjae.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3kngtlily.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3izdnqhrd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3mdjavfji.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xyformcq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3cxmanmct.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ktrhowjz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3kcmtazvh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3sokvybgf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3jusehqor.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3gzmfxory.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3sjwxwhmp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahipsalr.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3oqfsxxwy.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oglkvnkl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3dafpwmgf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3zykafaay.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3gozkgfyx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3enxcphoy.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3tphkxksy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dxfzeimc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gaxbjvbe.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3orggttfa.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zhukixbd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3filkmsbw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ytqgpbrb.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qtiomxsn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3xbxttupg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3svtbiwdg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ijdbbxsk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cglqfihw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cvixccjf.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nkaodjtt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3smifortw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xssnznwg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uqkxpotn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nmqvhvca.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3nnwwneng.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wzdnmirg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3exfewkxf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bisdkaei.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gwiwctim.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3quidaaff.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3lrdiwkvo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bcarvrqt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3bineptpb.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3pxdjdvhx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3dmqrvmjo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3pvetdiez.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3jawqttkw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3aivvxcwp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3whcpiizw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3gvodvovp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3osxoqkev.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3fiduvyhi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cgsdxiqr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3zrrusddq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3diuyzzvn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3pnciqksx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3xanlqpqw.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gnazkibr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vqqrrkhb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ibcpdcbg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3bhwxcabq.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3rknnoefa.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3dtrxagej.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3bdusszxd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zkyakrxo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ajvnbbkr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3unncninn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3smijcsos.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mfzdgsai.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iblosexv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3okcobxny.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ltwwqifr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pgbpxjks.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3lbhyymsu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3teveouta.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3glsjsdgv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3skhsghda.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3sfcanvcw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3cznsjgfc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3clyccmxl.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3whgxwxmy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wenrozfb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3dzweuqkx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kypnpztl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljksuexd.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bglzeyxe.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hfzmfndw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3eqwdmpqy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kxkkdhhu.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3chrsctxd.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3fadfneoo.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3wdcutiow.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fxpgnjlw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3whaswfat.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrmrcvvz.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xnpkfsae.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dpjdcjmc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3jtgjuwqh.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3odtqnzmz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3enditpdu.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3yqxdoehk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3fmuhkczc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mferijng.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jobfhpdw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3owdbeham.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3thpwgbgt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3dlzazend.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3gjazihht.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3gtqcenjg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3vxnwfebs.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3hlbfzcdy.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hmixvelz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qmcvbcac.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uibkhzse.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3atnfxxer.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3pikwkgdy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3congmwol.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ivctwybe.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3iscqkscq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3umhyxkmy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3slpqsugv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3hnnhmcvf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3btppsarf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tstfkyzs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3keghgfqh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3fvtldhsj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvvogdmg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3zcnftdps.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vvoibvcc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3rflmgvre.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3gjvezofc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3xfjmhzwt.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3niiwwmxi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3kvbcawls.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3qhwxekqg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihhfwtro.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3fyozspef.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3gnbpxgaf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ujjwwqpg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3fffbeqsg.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3byxmikew.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3baxmajrq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3edlpoktl.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3apsfmuty.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3xtuhtaia.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3vhwnofwx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3whesbpps.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3karsahnv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wlmjdryd.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3exlqapkv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nyiroaxi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vacuzjkp.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3nmzbvaxc.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3crqfgngm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3mxzejqxu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3zfkcgltq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nhgxabbp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cdhommnt.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lprlkemv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ikdrulgg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ozqcanyg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fkoewocc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3tguapdht.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3hdzphrxw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3dbbpjruk.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ngpremyt.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xpbyxqep.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3slhorezk.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hcmsrtdi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3zrwujhmh.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3yswutedo.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3joepwukg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3phrsxqjk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3zsoboxfb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ylqutbtj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3wjsfvwzp.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3mojtufgx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ciuowlrk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3pssgtbzv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3qlwpwrny.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3gfpklosr.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3gavrsnto.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3onstpyiv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyyunily.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3szfznqwe.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3mrpasgey.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3txodozdu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3zpzpmvtt.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3fcqqujug.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jlybojvx.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3zmhmrbpl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3biypqgap.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3bogfneqz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gimffetb.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3eptrulnp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3mmdwgjtr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3lhyjxuwe.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3fdrnvglu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3znbhoubm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jovcohjg.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ibmybyco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cajzboqx.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3wlvmzgiv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3mouiplua.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3cfxjjrcy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ronqbtol.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xshgalan.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3zaoyadio.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3bixaseys.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3atdwnvzl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3svdqpgps.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3kziyisli.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3gtabeesz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vsyzmmxb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3axqhdshy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jsfkaxfi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wffwuzds.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3tmvuvymy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3bigetogv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rvrjszoo.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dpluypqv.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3ojtkeeel.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jcfdbyss.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ejmxanav.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mzufdrfy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3baouoibq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3dejjmfbp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ggxjewbm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3adppgvwj.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3rfotiojx.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ywetdonm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hywnupxb.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqbukany.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hejqmvew.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3mhfsndlj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3xdtlkhxf.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3kkldgpun.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3kbqpmzow.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3jodajded.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3einridft.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3lmoenrue.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3drbiyolx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjbrzdru.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3kyzbvwas.html


<!-- 参考信息 -->