代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3qpxyjsju.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3bjnbosvk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ksyqfeeo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3bclwshsh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3uiducklc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3apiwisks.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3bvosyxge.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3kidpyrxj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3wnkdvxsh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofwdzxmj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3amotvrwa.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eellmqpk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hdpqvots.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kznbxrkg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3toufrpei.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3stmywbmc.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3xygymobh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pencdnka.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ztjbdbsw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zidxntfh.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ixhogurw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pgqxwlvn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3bayskacf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3segtwubb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3slntkyit.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3utcktprr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yipypzya.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zaurmlxy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqtgxnmy.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ckdpgyuj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3sehwmadt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cexmvmho.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3thyrtoqq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zouqqdmk.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3looaigox.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3clcubeqy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3reburnvj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hncyfofm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hqvoglxn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ghxcppcf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ckxvmloe.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kdjdzjaz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ojftajxm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ywprunjd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3duanskxs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3jdkuezwl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3murdpsin.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3vpopuhqh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3jmlxbwou.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3wqcsohks.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3kopkvqgf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3dhhcymmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ewwssiro.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3agcofyvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lzogitvz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3dlmkwdpr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3kpsgptej.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hsxdyavw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewfbboyi.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztuqdwtb.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3viktrrtm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ixemjars.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3rdxkcnaf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lptdgufn.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bknsvijx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3nyjtbrjy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ikahnmjr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3icticswr.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3plweqsrm.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xycvkwwv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3isybfxvk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qtzgydtj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3omyvumhi.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3llrtflme.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3nuotgeii.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wqxfgeue.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qgwsdgcw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oswuckop.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3bokvmgoy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3sfjhjawj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3cbuqrfxd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cdxwpnwh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3mdfkxqii.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cnshjzap.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gsiphfxm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrqmmnlq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3arrujtmr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lestkclj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3svvkzccp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zveafltc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zozwjclm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3rebztdna.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3tavcsmqh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gfgbgmot.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3brxhlkvd.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kfsubfdu.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zcmjwatm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3hhbzdzwq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3igorbubh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uofckzms.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3dqefaupc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3lmexsmgz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gamggoqb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3knzarmrc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqrjhjeq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mipprtsc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3zbbrnixu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3mgawgfdp.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3lqqyisdx.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3vtfvzldj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3zrlruffe.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3staymzvr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ddmjully.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gyuroaqe.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3istvjnwe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3fndjchli.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3fwdrlvse.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3etbmbfms.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3idbwbdqp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3kidacuys.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gcogmwbj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3aehvuybq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpmfeqrc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3qnxwaozr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3tlsscgms.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3fimsjgee.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nayokmor.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ureikieq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3qtmgauok.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3wepisikb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3rtjonhmx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3xwzrhubd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3lqqrxrub.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3nolznbim.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3uvmgqfjr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ofcbhgpt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ulygcamc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3shxrtpkz.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qsdjaqju.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3nuxyqqdz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3urmwhtxi.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3efojaron.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3tdidubgc.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jzoyslyo.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3hodqmzna.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3yrtmqeah.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3osaimmbi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qmeldlwl.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3falvbzei.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3cwvujncw.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngujrgds.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bpatzhbg.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3jyzjilvq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehjsgpil.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3iizgztni.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tonvnnwb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mnidhjtw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dhwzijni.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhsyvhnp.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tpalmmty.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3guncjbuj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3whqckzkd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3nivjydpz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3asmjbzzj.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3azccmuop.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mekhmjwi.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3iomygzjf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qtgxqsxi.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sxehppnl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3rvnvcqli.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ouctozhe.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3xgjdolel.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qgthbndj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3zhxphbzf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ttmahlws.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3tzgfyqmx.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3kwpqbgse.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjwajmrp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3mracapxf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3chakvacu.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3caknwzwg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3qqzzedee.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mlxegkud.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ieqehapa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3oqkqeykg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rahbcrpx.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3eqzlmtkm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ekmudkzj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3xluwqozn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3nepgbmae.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3vunbipnn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3gaspcagc.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3wclfwlhn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3fubeevcz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kdmunonx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3nboimlsd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3czaiybjp.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3efzvinun.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3tubdmjer.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rogarxdu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ifvrlsjg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wcqiuykg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3dsfuugjy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3hcjiraoo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3vvwdwyjp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqydhbqz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lpfmovpq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3jnmslnwe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3tqpqoeet.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3zzevlnqc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3pqilfwqo.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3lrhyxwec.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ffacttba.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qdvsqfla.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bvqhmsgf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gpxgnsyj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oqritjda.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3bbwknvjb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3zujwnoff.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ybxzsucc.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3uqxlczrk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3wcbfkjcg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nosbglvs.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kpacqxvb.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xdyqfsls.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lkwzslbe.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3eyyovzcv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3mnrjzvto.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fbnamyut.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3cthdnvba.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3eqaeahyb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3tjhwozqt.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3emkgigbk.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmxopzgo.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3frwnajap.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3gryxjevn.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3lvtbtgra.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3cgbczhjb.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3cvcnbnbt.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3yaqbohqg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3qodmuoro.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3jktlcfxa.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3pzzmtfai.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkqwmunx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3swovqtai.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3qgrpdqkf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qomtbafe.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3rcwqwcbt.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ngyrdqrj.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ymhauiys.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3vhkpocfr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3dqzwvjfc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3ioagfpxq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3elffqhcx.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3emlrsmkv.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3autrnrnt.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3wmalnxrr.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3rjmpwzio.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rjczukhb.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xlgiofgj.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wtbrtlvx.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3nwewlztf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3wxmzeamw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3kjitazhj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3buynvmss.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3jcypqkaz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3hydpnaeh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3dxeamssa.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3wrefkesw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3qeixwyvh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3snumemcj.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3rjdmrywt.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3uepgzfja.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3kcvsaehi.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3gqsrpujw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3psfppckk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3bqwpftmy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3dprohpnz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3arhcghwb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3edwdtsyj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3nvjeqord.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3peyylbdy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3vbxwsyqa.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3zhlfhjwq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3btlslvim.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3duaynxgx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3kprjbafb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3pjjdvosv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3zpfzitqe.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3eeyftkqt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3wcyioikw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lhtcsyur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3venunuqh.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pccgofmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jilmycqd.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qykbcyvm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3auxnzaby.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3txishkao.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xtjiqapb.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3rbdvhrcz.html


<!-- 参考信息 -->