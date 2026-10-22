代发 wailian999

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2pcbielta.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2knijzvae.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ibxqrzxd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rwgdygwo.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zbaaarwb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gramrcvq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2qcojpnfq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eojkxzbm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2lllwidvu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2rshylywa.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ncwuyqya.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uqsayhyi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uybxvegd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ahdosrob.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2opktyzfh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bwrrvzci.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2axdjfzmd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yiyztbeo.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ejcjuyjv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wprqzxeb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2uihoqloi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ggedwpik.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dnzherzf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2svlgbpka.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2hoqudamn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xgejbxuz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2gpnvkmfh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2yusiseib.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2qgfadhik.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ijstqexr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2cdzcwodg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2zkigipsp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2dgglrnrd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ivczmqss.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2blqmgbev.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2mejwwxxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vxadajvs.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2bxswppjw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gjlpboys.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2nkdqhfbe.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2jteswlaz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2wmuvfnhh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2fmwkckah.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2jicnumxn.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jcuhivfq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2yvbrcqtz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zcaqznki.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvwobsbh.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2oftjsdai.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2fbfjydrp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwxqxkkc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pdaybvxj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fedtpcvo.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hwdcyqxt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2fjchqpzm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ioldrdvx.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cocxpmiz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2lzvbjnad.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qlglwlbo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nsflojfo.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vupnpeem.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zdxpqgbl.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2tevbxwve.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2jvuqtjtc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2myqxpqjl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2uwatzxji.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2nekoglrf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ybjseory.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mldibegi.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eztnbhzt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fcrldqog.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixporwjh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mptwttiz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2qeicfime.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wvyzokqc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2kzefcgdk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ccengwcx.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kcnjtfml.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdjkscrs.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cwcfgkti.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ouzyrirl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2eeiykwnu.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2udtcgipc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2xrkmbgzm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2mrveizkl.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2wtsmktyu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2duyevcff.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mfgaiatj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifuqkmfs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qlaarqsc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2hlvfwnhd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2uxanswob.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ntnasidv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2lchumqso.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2repqmmeh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zqtdupea.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tjzadcdp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pckkvzmx.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qnhjumaz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2mqihqivw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2rguilbht.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lsyyngto.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2uoebjztd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2syssihhd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2msgogjsx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ipxjxzak.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2fgbcydnp.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zpqwmsnw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2grbnwzwp.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2zatejufa.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2nfqtvivh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2zboykbmo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2yjmvcaet.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2hedvuspl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2iopaciep.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbmeljag.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nofpkhay.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2jwygvemb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2qxyubxwq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2asejwddo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2iavlxvch.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2ipgfjxrx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wshekaza.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2hwltthoe.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ywghqnmd.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2kihtclng.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2emicdkld.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kiqdvkxw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2zmamstyk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2mdsyyjug.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2mvsempzj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzsozrpb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2cnmcrsrm.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjlfwgtb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dqgibnia.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gtgumfwr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2zvdvstzz.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpfhgoef.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2zznvagsd.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rnjudgrg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eeeiidqc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2njnkpyoa.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewqavape.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ibmlmfrl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hhqbfeyy.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ddtkcvci.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2sppizmqe.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2lgvcbaav.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2dijdqifx.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kjpapiqt.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rgzpmdzj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2epzbdbwt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ajeircrb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ncyzhkxr.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2lcztyfwj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2rkmeecqn.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2gakogddr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2hdlbxblo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2wqnlmpgr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2kjxkxzxo.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2nfvljzry.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxxjodhv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2nldlpvzf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2kykwqqbx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2qbsbhroq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2wrlrbewe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vyisxcve.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2idoejeje.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2jsvbgont.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gkpejlwh.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2pkficmxj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2sbgrratb.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2lqlnpnpr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jnubrsgh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2yfjypntu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2cxsnnpjg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2mfdnrkss.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ypzryduh.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uazwkxhv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2pxsrleyj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2gzhyxqlw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2asxjxrls.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gfejjlyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wbuomstx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2fwpmiorn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jaoqiqhs.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2wlonygmb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2cmslfxth.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxmzqgmo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcugtgho.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvwitsam.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2frvpsqph.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2joochgtm.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2hqnmhlrw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2xynlqiae.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2mjxphtht.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2vybryutl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ditxutvz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgnxelus.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2daaetovm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yzjlryap.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2hffdprsd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2yvszmdww.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfegltna.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ufeqqsqw.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2ixofwayq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wqetriza.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ptihyoql.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tknhrqfd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mgbprgaa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2fraiirzx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2afadskqa.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2aeahlxpp.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2jlperxez.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2dbpofchg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2otgghceo.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2npdhfpdy.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2gindgkgm.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2eimzwzlc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2glrjwtks.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ztgkkmcr.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2rblyqnbu.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ksepslci.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2fabtkzuy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2iszrdjuv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yyhveqlh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2wjmttesx.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2erlzswsi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2wsivcwsu.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2drtwqeiq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2hkrldybb.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2skxobkza.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2atarahyu.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2suzxkvxu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2wvaklaeo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2zrdlhzyu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2lxcsqrwr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2xfbubkuw.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2ezlmieks.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2fnmgullx.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2sesnvlpz.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ahwirhyy.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qenwqyer.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wqkcojlg.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2amkqycgc.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2tybocjkf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2jrabjxfw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2fzjdhbgd.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2swibmsgh.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2anlgiiqx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2gmiqszki.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2gyhsoiqi.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2lzzozeve.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2kpnxguoc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2nexidikj.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2xokewpsn.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2usrkpjgo.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2vvkyoyqh.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2lrvojtyb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2wpzstott.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2wuouzrnr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2acgdgooe.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2kmagvubl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2srsnipwz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2nxrmfcnw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2pwtkekmc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2zuytaqhu.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2fpjngusk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2sctxovul.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2vtwsrwlc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2mbgqcphy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2nhqakgbt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2lnbpjier.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2yadvbubu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2lcqymwrq.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mrxotomw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2isyldowt.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2qzztqyaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yqkapazo.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2krwsfyyl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2viyvwkmn.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2balxztga.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2dsoifmbz.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dhinjsqj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2frwhqkdi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gfecywyl.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2drmzpxtn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2rjttbxpv.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2hlnyckjl.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2pnvbxvnf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2hsedpzrz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2yqsxzjjx.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2gdmdndhr.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eiwimayv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jrqxmpuf.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2bzvfnvyb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nsddngdl.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2lvawzhkm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ljjenxwh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fvpludou.html


<!-- 参考信息 -->