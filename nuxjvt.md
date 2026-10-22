代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2octljuwx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jcbyfvne.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2imaqthta.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2zzjnwnrp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2djsatfij.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2klthouzb.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2pmccmzvj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2wafrisnz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2yzedkczg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lyzryjqf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qrdnlbux.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2spzksffk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2qhrjfaqq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2jetajfsc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2lktjvgns.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2mtecmyrf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fzjoneey.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2whqjyzmj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2letzzcha.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rkdoecew.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2lxwtctta.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fhliexgb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2mrnvrloc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2tcmuoryc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lvmuqain.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2bxrzipvy.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hwrhekuq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ajuedcif.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2avrhuhpd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qyegipbh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2culpjzms.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jeyjxfvd.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xugsxylc.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2vsavkelh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rqjykqmw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ljtlwjbs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iesivqwg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oexkqdgi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ezukvpgw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ogsfhchi.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kjijqryg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2knjyktil.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2jrjdmgvs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jzaouche.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2krgdhgrj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2aqhqparn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2olgyhkxl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2fcyreuwt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2amffswzb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jkclvwqr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ezekbfbu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2vvgaupmc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2lmxkuiyo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2uorciypu.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lpmqvfhx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bnjmfxdt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2naylfjkn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fcylgsps.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yfgsrsia.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ldepghhu.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2qiooktus.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wjhvjygn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rlhzwozd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mykbdowh.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fscmipzt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fsrmoywc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2pnqtmnsb.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qwwwznhx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2jvosrmrl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2yzptwljd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gdqgjjxp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2feyuwfce.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2klntoery.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yggxgofr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2cebgnpoi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mjesniht.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rdwzomqi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2myvarvvz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2kirxhpjx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dzfmwlmx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lyuppfio.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2chwlltsl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kcxdlsck.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kkfoexob.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2gtxnkfrs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aowmpifm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2hlcndwuh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2rblpgcwq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ujudqjid.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2qhrazmsh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2jlsbdbmt.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2hvomxrna.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2nexgxigp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2pqnpturm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2opbxuuyj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2yyzpqhqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oewcziax.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2jcmeyiek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bzcmcpsd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2lslsufxp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2gglspcwz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixxaxmed.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xpodybpa.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2akiousri.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdvesfbv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2bxocamzg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hkynboek.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dlldugnp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dvexbbde.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2gpqzoint.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wdppirxw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rwynxkse.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2irkcferl.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xneijfyu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2lzwrrlgs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vgeerpca.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2prfosxho.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2mzqkfuge.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2inxpativ.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2hromohoj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2amzbmirm.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ppzaijwg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2cedmmren.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ssnimxlr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hlgcmkhh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2eyvfnkfy.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2yrcelxec.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hwttqqky.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gzatgcrh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rybscknf.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jigulqsf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzyhsuhv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2urgerxex.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2byqdqeml.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2oylfmdwm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2lhnthwsu.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ouziypwr.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yplwgopi.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vpogfufv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rxfrjkfz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zteshikj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2rimghedt.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dxsczenj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2rhlsmcbr.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2rknvdwwd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2btbyjvqk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwdhxgyw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mziasppx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yqrsrmma.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkzwlayv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2pfnmgwgh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2klbgyhek.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2jibcbkxf.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2tlbsjtgd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2thjtmtzr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2igxkkxcl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fhmbochm.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2obdwxhom.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oaxpziyd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2wcdysjav.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2fmgmlikk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bobrrvvw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2negktolu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2hamxaflq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2rlwoezgp.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajydpwrx.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgksnjzn.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ympbahsf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2vjzivlkr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2jhuohqdb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wexoufbb.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ddiifpya.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2lfxbtlbs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfjjxehf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2qcmqhdgl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2yowdhzey.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2lzjbsuvw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2wlcvjaiu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2rarmyzro.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2tivbszwn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2nzvfilru.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2axvwkewy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gzlpxyej.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2uxeqqshb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2utamlomz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2mnntftad.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2uenfbyfq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ngcvyslo.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2umoyyvaj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2bmgyyhqu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2dkavwmcc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eogfjcbg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2swknwqbf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2liqhrfzo.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrrcpixw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qxhvbvlc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2mtsjfspy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2pmvoshvf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2azlbtqro.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2yfpdmtxu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2aldxqvmq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcftsjos.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nrcpovzu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nfazvsxn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2axpnjlrz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2swjzcgmf.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2odytfoex.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mvfgmlcv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2miptwfhn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2evwszxwz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qmtfjpig.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ajpgqtlk.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wfydwucj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2hecjqday.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2jwxqufab.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2rfdsecwj.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2vvsnkdko.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2dkcjvoml.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2eqxirzxj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2uxngiqbs.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2sysxchml.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbhpulgi.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2detefnoj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2lslukkqb.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2kwazdqfy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gztafsnk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2qwxgtgpc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbczfbkj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ffepyngk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jdcvwvaf.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2wkwbuawa.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2jqfdbsmj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2azwqmuzk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wkxmchlw.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2wrsfnyad.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2iybuiqol.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2czeubhmu.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ydrmpvab.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ghlbkvzh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2gumkhvsx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2blqmxjec.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2yhgumqbl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ylenelvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hgqbiqfb.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2nyydpvux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmroyblu.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2dldvvwzz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2vxcuujxd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2fmypprnw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehaygzhd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfnmmmnp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xciibcmv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2fxclxsgo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2nnhmeuxc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2idkuiitq.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2iitwpdqy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2jysefvpa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yhxfdylr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2plownnuv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jniztenw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tytvxmav.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ugkalbhj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ndqnkjod.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ayzjbkhu.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xdgxlgjn.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2yeufhqbp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ykujswki.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2skexbsos.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zqomqgau.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bdbyrhzg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2rvbemopm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2kwluukdg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mlxfpzkq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2gqwbdmqp.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2quqpngbz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2fpgeumxx.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kyubjzla.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2trtpxtws.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rcjiscmt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2vkmgscmj.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2afzemrff.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2mkybfpuf.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2xscnomle.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2fccjpxfw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2kinzaosx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tldcewoo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2vmecwdvx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgijxujb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ctiotihi.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2eyzgucle.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxxdaqma.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2wuznuflk.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2vuvnustw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2sikxrfdy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ckadumjr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2uoalqisi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2naqtluai.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2kopjnuwl.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2fyeafftk.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2diktbezj.html


<!-- 参考信息 -->