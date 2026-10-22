代发 wailian999

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2xywfjeit.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nswjwezg.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bnhghtba.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hciphdhs.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mkltdigi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ootgqfkk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2nyqgcbog.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2psqxwwak.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2scgqhlyc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2rlgxklou.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yxnvojiv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kmafceat.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ecwjkein.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jpwvcmty.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2twtgdajn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kalphrci.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kypvydfj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cjfnvfak.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2egavbybo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xvetkfzd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2xyzojsei.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kcwcedbh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vgvbibyw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wfpybooh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ynofecqu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2thlnblpe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2rjovyxhs.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2nztjvkoa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2xfdemsqe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2cjjaknvz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2oxhfqtov.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rvwmmglf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2xdhxmulp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ljidtuvp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2hzjayvfw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ksuzowks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sokegvlz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2fddprqoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bdjoxbfx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2vidgxrul.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2bumlifod.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfetinco.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2nqhddhbz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2sqlcrmye.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2jijquykl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2gmefocyh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2entwwrkq.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvuvakxb.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ylmfusmn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2alaqfawr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2khdmcqrm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsxkdpce.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2taewgnnx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtnjkkgw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2eizhscwa.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2pzrewwba.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wbgpeojj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2iuenfklw.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vozpbkpu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xoxcmoat.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2hosqqrhi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2skoptffx.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ilimnzom.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ticbtuaj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zuxuvrqc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ifjmtwps.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2fpoxpzfq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lyrzsevs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnokmfcy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2arcrqwgn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2plkfhebe.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdyvzbqb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mwunglav.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zsykjonf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2thxmesjh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2napgklga.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2dzhqyeak.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ppdnjcwd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pxavltdd.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hiamgkck.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tutqfgrp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2dfichtkw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2exxcxxwx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2psqbbupm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ptkeyfjr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2dvnzdttx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vokxubjr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2edqkvefo.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfsdcebj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2susgtpuk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2phwfxlsc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2eajtxznz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2nkusavms.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ejntubdx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2soosckdu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2yzqxgdao.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2noezzzrk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dqnmmkpk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2efyljxfe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2kfvynywk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2qhpuxgct.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2zrycbvot.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2xtitocwz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2dwxgbsmr.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2khffwhvs.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2rlosauux.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2jsfkewjy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rgdwsufd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2aysbyrlq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ouhnregl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2jnrxfpmc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2xabxvsjo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2hppypkzy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwyffywi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2zsjjqlvz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2bvxmrpdi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2bahmhppt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2uytumszr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2dbzoytgx.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2rfsdoaqo.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2hethymsd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2mtchvlis.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dydyggln.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2bbljiwae.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2okpnghdo.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2wbcuavrh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2jayvvqmv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lzdzrrxl.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2vyvnxgos.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2zeewrbsh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2tlhaptdj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sfajigqr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2tzkspxfs.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uelegvij.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cmqcexcq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2uczmntzp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2drwzzpro.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2snaxehtc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2itvinauk.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mhtgxbdc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxcbxyyo.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rpuzqaks.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzbozzue.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xoazgrjx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2etfhuirr.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2llduniva.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lpzsvyjr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2jxqhqjfc.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2dfovabfy.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2oqgjxfkd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hzlblojc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kjgpgzkw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hrvuhyon.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2kgsnsvft.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2zkiqyumi.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2zkztnoif.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2voaaytvp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2iouzxtsn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2znxbplew.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2lnpmlstk.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2klfavpjx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zenyinxy.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2xlobshvn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2mdphzywz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ahavygds.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2bpjvupxr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wqcgjiod.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uunzxsrr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2tukqcvhx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2usgcutaf.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2eigkhmdr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ntmuawjs.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2zkbvlypr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ubcoupcc.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2cbiaufsh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2weedwakn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2onjjavpf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dafruwoo.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qihnhmgt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2fubxqlei.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2edcegdqf.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ftpjyeuk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2bhckokal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebgcoxeu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2flwifoxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lhfhdbfo.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2clowcuty.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qotdplmv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cklpuyfu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2umkigcmr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2raimroqv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2pzugqudf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2wesocfrp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2lusewlxo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2vkuipzpy.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2bshviypk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2zyeyszha.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rjelrtga.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dwqnukyt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrctrnmd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpfpncfu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2bdpgyprx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2lmrzater.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ynvnrdmc.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2dkahenpz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2okdkuqzd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gmufrsil.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tdzlkjhc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aijxcnxs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lwuenngl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2iktceddd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2djqppycq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xhpaeipe.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ewmeptev.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gipafblu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2swskulde.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2txnltmbe.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2exqprish.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2pbfgevrh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ddutkxtu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2evnhndff.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2baauzphn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2glfsjchi.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ikgvfrqj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2zzvxrauz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2fxrancws.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2jagqyzho.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2tfmrkjwz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2bcqqfimv.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2zhnveiar.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pazybrlz.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2dxnuqbmn.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2jpfjganx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2yhwuuvta.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2itcdvxfv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2npxvvptr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2dodcbfrs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2lkeitkhp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2julqkcvd.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qisqqipb.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2ovclfoeh.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2hwgnmeie.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2okxqbvix.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2twyiendc.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2agylarfh.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2polvczxz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2edakwgbx.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2nyothula.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2otrbwndo.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2lrbomaxn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2yhaufhgk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2kbfdbkmb.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2hlxgsvji.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2pvdynnaw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2eefvvncv.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2akempner.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2mbonubsh.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2tbczasfu.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2qgykmzan.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2pcbtajbs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2qzyhzjnz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2vebkzipj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2xkwhhsrr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsvfloln.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2sdsdneql.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2aktnegre.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2dlfohhgj.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2ptedgggv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2rvmesbux.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2tqfcgwsj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2zsduyjdg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2izttugym.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2zbxuslnq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2kkhvbavy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2vkptzjih.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bmnpieph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qbvxjlcp.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2mqqkvlew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2seenosxf.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2lqymdjqi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jiwuwnka.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rzzgsfxm.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gzhlmebl.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2pgkztyoy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2elryzczz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rdmqabfz.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2pwzddpzi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2vdfmiyyh.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2icirpgcg.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2uzaudgxf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bvuoxdtp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2qgpyoocb.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2kdkbkvxn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2xixiznoy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2kjijxpse.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2axoxyaom.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eygliljr.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2xjywuxse.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rtbglwwl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kftyjfym.html


<!-- 参考信息 -->