代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2xhoqybwu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2qvqadndb.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2bmuuppss.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2licmghuc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2izvfrgte.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dgqqiabv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2iuhrbvpe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2adgcimbw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2mqbozlei.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ubbdhukm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bfadtfvn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2tbzpsvve.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mwxmcvsg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2nmilxwkt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jcxmasco.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2inaoxcvv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2sjlgsnbn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jwrcsawe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2tvipczou.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xgiwxmfg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nbxiwecy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ihnzwspg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2illgrlee.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dqhqmqct.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mwufbhoe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lrrkpeyu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2nopkcxjq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hzwosohz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mwqrqmbp.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2voabzhac.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2btzwuibd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nujpgehy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kvskevdz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ktwpvlsp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2srldbtin.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aasdprqr.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2occwqngy.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vnfkhqnw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ettzzqdx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sjlmeafe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2magcrugo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2eivgiwcv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zgveqnsn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2idoxdgnt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2dohzregk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ybnapdhj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2cfkyyfft.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2zxkzxonu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2saajmbtp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2trflznkk.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bwobakur.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ccsyazft.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2lkovqsvb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vbxantpo.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jupubsct.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ylhelbyf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2qsfxkjsq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lulilpht.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ubkghgwh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zauywjxa.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ahxctaop.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lohjtmve.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2tknpnfcr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ypycgplh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2orecgwpm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2xvuvfoii.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bsbdyyhi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vywusxul.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wjjfjjag.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ruesevjj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2mdyrorct.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zxebqvxa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xnbswfdl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yxhgtzoi.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2zqdeywqx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kuuupvqw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2mygervwq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mojcmpij.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vgazxull.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wynwtemq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2wexnuefp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2apqmtula.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2bpzrjwss.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2aaawilfq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2xxpphckt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2opnewxum.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2sqwftton.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bkwedsbv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2hmqfhctn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2bmpiwwxi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2uwwtrdxb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2tmyyjkmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gbgnpxyn.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2hkvfwvht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdkyncfa.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2yzddmeqa.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2vzwaiifm.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2utyemner.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2midijxxz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2djbsradp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2exuxblrs.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2mrlfqmir.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wweglsar.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2goacudpw.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2lntmumhf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ycsydnya.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2sksjuhot.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvkurthb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfssujfc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2slrosdkx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2jtbxnjkl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wkdjgxms.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qexuyzlu.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2wbwtntki.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2dzafujsf.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vncxzjfo.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2kekbtnql.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ffzoyvan.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2vmhdifjp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2xxjcrerh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vdzzcorz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2gxquwpri.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2pelioyvo.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2kjajbrft.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nadxeoum.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rtyyqswg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nyiydgum.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqseegts.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ojlqqxqf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qociazpl.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2blxqrpec.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2lcwvwnqp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2kbdlwiyu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmipnqxe.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vowufuji.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lofatxev.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqeonhqi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2zpatlwao.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bzyfqybj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iddszgem.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ushhxnkp.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ujblmyec.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2aovkpdfh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwcggdbw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfumxlue.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwqrovah.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2zuclizzy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2btiyzmug.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ldfbpygw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2hjlvxyiu.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2uwriqjtr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fvlciecy.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ghkceujh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nhwsnfiy.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lnswrvjj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2eqguchbc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2xmphzyav.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2azfenpay.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2dchimxvo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2mmygsukj.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2coexabqv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dusoxcky.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2kwwbxqkh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2eyqxwtan.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2vryksvxq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2xnaelgjw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmzlguzs.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2bqbuhrdz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2yqcayeqv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2dxboqlry.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2djmgkjmf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2nayweioe.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehibhxdb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2kratnbgj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2godbnnuu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wkmzmdgv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2bgafmxso.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2cftbukeu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xmwopgwm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2rxypjubo.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gimzrbpi.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2adqyhfur.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2oisckosm.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kxnucjjy.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2kzbdvauo.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2mptxuhvr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2beuxvtnw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mowvyoga.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2acdadnlg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dpwqttam.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fqomphpg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2faqvcukn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2bsgoklmq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2pskvkclz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2pzfaydhi.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jbmlqgwz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bnrjlwbh.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eexjlitr.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ceielbqq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqihbbpp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jiwktsor.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uktzikyq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2oxmlpjuz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2cmcbapnt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2tblfigxm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xiinwtqi.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yyrdxift.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pbfgyldf.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hpulhssw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ohpzhivc.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2kqhwygzu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2rqtqlvdr.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2awhyjmqu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2kszqjclc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2cmgjlang.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2cholxzez.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2qpimsaos.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2accppvmi.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2bawqvebb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2jkxymfgk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2hqpazhii.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2juqhubac.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ryfgjzas.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2scihqnmp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2upzrpkho.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2fiupkyxb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2zhetopsg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2dyhtggbf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2tgooxqhy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2pwnqclsf.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2pfzbpmqp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2yooeself.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2jepvraal.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2fcpdfdyl.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jayzjagw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2kiodewlv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2whvhkkjq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2pncdjcmv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2bwydcfwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbfimgjl.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2zexymxnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lgurxepc.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2weevswpo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2pymsqwbx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iukguitm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rplkmebn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kuktdjdi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybfnigei.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ukmpqiid.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2vtzjbihm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ulysczea.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2lzlciege.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2hbgaojoy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2onebtovv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtspikee.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2obviisvb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2homsmrli.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2efbrrske.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2koutusdv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cmxbtlts.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2sxjvawps.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2fhegswwh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2enwjehwn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kqwwqlsw.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hjwwiikw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lbreogjs.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2habryfji.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2zahhwhjm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nmhmcwzb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2yrgymvvr.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2pjqdbilb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2fjajjfgc.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xyqjjkal.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ceinflez.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2uysutxid.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2kxpbvbom.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2stxupuon.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2lyfzmydt.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2tcmlaecs.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2vojrntmo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2fvofcoet.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vlfxptsj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjwwoeyt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhtirgzd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2wgnodesp.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2cobafccb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2bqishpbj.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2psjdtlyt.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2jozrzfob.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2tzpjxwrr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2retcgnxo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2grzyqnxt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2evefkdyg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2gxzjxevy.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2cmusswje.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bkrreaup.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2eqnmivwv.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2fwxgbada.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pjaxnpzy.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jkxdjlvt.html


<!-- 参考信息 -->