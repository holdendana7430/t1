代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kdylpasc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lduxoftk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2qqbphwwl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ytyvvlru.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2sqeajnaw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ernsphxf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jrbuofqy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2awwtzubb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hubyczeh.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tjrnhndo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2syvfsgwl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hsqodncp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2opkqbwqx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uqmkejpn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2yrdaxsnm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qhadhxrz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2kymiojkm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dguhriqn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wbureieh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fusilknn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2hyoebcra.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2thsuwxoh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2vjvabshm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2noidqkdd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2dphmqgwb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2amzzmxvw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2tqadhokk.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2kksyqvmw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2clhsorjc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2bkjqrhrf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ynlhcyqi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ebzymogo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fguspxrb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2thikbolb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2usrokxgw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2tiarqtmc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2dlwbkegn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xuqcztxp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2kwrkxdko.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2oztwlcjj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wopvxbwk.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2nqwebbid.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2iksedvge.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ljtgymcg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2zawjqzff.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2lntvwyuq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ndqixfwh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bxrqkyoo.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2qmcudnfr.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kpxafcav.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2imocoxua.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vqzwmxmg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ermmvyvx.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2pifsqtqy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tklrntvd.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2aukotfay.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dbxjtrjz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zjtehxli.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2kjgbplwi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2idvrqbxv.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2tqjisbev.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2gprlmleh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2hfsttwcy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2culrixbe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2urlgggpf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uwlqkmna.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqaoasby.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzrixklr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2thmpjjfg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nerkhutd.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nzmfceqy.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2weqzrfqd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2dgsuvpxr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pstnpkqi.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zywfooll.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zctqcmkk.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cnbgahnw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2uqfaslnu.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gtbpzbku.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2txufwwlj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2kerkqywa.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2prslzhgl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tdqygzga.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fdcbpcbj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2asohnvud.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nygerauj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2aupkpiih.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2bnriovay.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2kfeqnfbs.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2qnxhbzzl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2mkjvuxtx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ssyyvksr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2yxndaour.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tpvngelj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jrxjecvd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2rbuavbts.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2zqrguvce.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2tfzmqdms.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2tixbzyzt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2xkuwcgyo.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2iitiqupi.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2viqrwynz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2lerknwel.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ouceiinl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2sgvmcfpa.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ggveafzi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xskdrplg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2nncvyoux.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2rgpsgevh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2phbcyxgc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2prxlekrd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2udzkvmkn.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2tikwxjza.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2vyiczept.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2eaqyaklq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2xjohxvco.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2xtnhbghk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ejjnprwz.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ocjvvswm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2qkqfbhtr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2abowczgu.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2dkmrruys.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2adpthhep.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2oyequogf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2euaebzyr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2kdxjthrm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2kiodkraz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2utblyxfn.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qswrgygj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gjslzdbv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eajmnfxu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2awkbbdtu.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2cdsxcctz.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyyquxwy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dtjzffsu.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nasorrzh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvfrmmod.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfngzgdj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dennrfqq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oovmkpyn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2flylmkel.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2naynyxnq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ncfndfuo.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2wmmdniqr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2djaljvtl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gezfimwb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gncraucq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2iqqyrokq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ppphxzkx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2mrrbiipn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2tjrgxoau.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2syjriwrn.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2quimpoin.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2qfpgnmzo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ybsfwbzp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ntjmparc.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2rbeqddfq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2vutazazs.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ztcithqs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2lwqtbhwa.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ujkfqbhq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2cuhrsoml.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2afbqufji.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2tlutwiyl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ebeqcdrx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ftawfxdv.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2wcnoqxmg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2fnaaijuh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2bkpdfbsd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2gaipzqak.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2oauapksa.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2yfwwibhi.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2rnzsbmgf.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mguctffz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dgmxngpa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ytvgwtyv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2kbocnthm.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2knbbtzit.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xclibrvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lgobzwza.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2elgsqfpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nbqyxyhh.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2okkzwyqw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2goddektp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2kmaxzmbf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ciniqiad.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kdojmtqj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2bqkukwdp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2vahucacv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2yywlypia.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2hemvhhtn.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2isrkfddz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2glzjqqnr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sdwritdk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yhjsewef.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xifytlrh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2diglqiqn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ohwvskpj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2zbtehaow.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwzllhij.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fuitkjtt.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2onplklqw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jjzvchwn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2huwhwttv.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xcebphaz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ifvvixzi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2dbubolya.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2jdfdnzzc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jntvipjd.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2bpwbntjh.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2tptvmzqf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebloenlt.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2orqgzkgi.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmijaptw.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhsdgtbz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2mdgpbbbn.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2gcggljur.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2wrjcfmqw.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2gvgitkgg.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2kkbmfiye.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ctuzttmy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcykxmij.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2cumhqomw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2dxulsfea.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2sssfirpd.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2gxybwlzx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2jnvgxexu.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2zrshlmoi.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2oscbrjzr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2gitffffr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2seucqpmt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2piddipuz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2dvkkipvx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2xnhqgius.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2stawtzyq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2kpvltkel.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2emirwfgd.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2plouwmfs.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qpkvizfg.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rrztuesm.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2fhpedxjz.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2uccyufxj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2dflyrpkw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2kvuyxcsw.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jykdgais.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2djjasyhf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ddimhtib.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2uxfntcph.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2rfvlkfov.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2rmfzepyt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2owyzehen.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2vwftieye.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2fvxsadsu.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2hinxutdx.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2plpyutlh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2mmlgpdsw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2idyqhudi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2vaexxirj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2wgedouce.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2kroxbiuo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2slzbgwda.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2veatryvg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2fndfdpks.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2ghsuyzjl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2kufuaabp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2asqjthkx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2qpjeojrh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2msspicol.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2ihfnlhhb.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2rlwtrupp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2sedaektv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2exrnrblm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mtwqztoj.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2htfoluec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mczozmnl.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eogjloom.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2cnepatrd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hctveone.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ofyebsdp.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2focsqztr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2radzhlix.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2srjylanm.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2rlvgkcej.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ffulywvq.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ghjikujg.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2butfxmjq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2vxujasgw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2wwhowien.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2acqebcin.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2ruimsnjy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2lreqpbdx.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2urxgaakr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jgonxecq.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2aaflzrjw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2furcaqbi.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2sgkjykpz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2nktmchsq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2sfjmdvwk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2cdewjrle.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2xcgruibm.html


<!-- 参考信息 -->