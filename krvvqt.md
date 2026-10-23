代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eetngzfa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3agynhene.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3czepncli.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jetmypjw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ewudniyq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gzreytij.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3letlhgnk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hskgzwlz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3poajeluh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nmwrseyy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3pqycnmte.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3fslxxksm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3rjdltgjg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3nuxktshw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3rckynhes.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3jqmwvogo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3jcyrwsbw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3jvghmtsf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3fgcsxxff.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zudhupja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ibpxrokr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3kezdvbne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bcipuque.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3dkwqntpj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ebrgbyxr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3hpexfnpf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hmmpadlg.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3sufspnhx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvxdewyz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3puuslygs.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3wvdmrfqj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3exjhfqlt.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3suhshccq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3jkcnlmct.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zvjmxyvh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bezuaush.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tglatxmx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryxeuhsx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3wojamtcp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3lkjpskra.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pjztukey.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3nozbqgvi.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kxaahrvu.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ctsxqvnd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nvicpcks.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cwbsiufp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3kgpjsvrj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3titsidxk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3oqsgibhe.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3umuqfkak.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ghzhzgwq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xzvpxvek.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bfihqcce.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjwjsmrs.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ecuohhxa.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ealnabkn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tyuvmkze.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3aiqpbfku.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vjunujtp.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3vgwawdrr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3skwoppuv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffwasfac.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ulsfskmz.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3thrlafae.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmqpqrty.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3lfnhpjoy.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ezyyvdjp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3cmfoomvp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3rfhdxqnf.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3qzaecdpc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3scjcwiap.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ihxzvtsv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsidksrw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3crahodny.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3worxzuro.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3rhqxifkw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3lydctfdf.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3tvptwayt.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3msadugbm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3brylkqhn.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zwpdqvdi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cxiqvvle.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vhmyyiwb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3fvjsrldw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3tzuikcbs.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3uzamkkqf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3rzcdlahf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ufnlcwvt.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddjnnbcm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmksajii.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3pjbrmptn.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zrzpktho.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3djfretmz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3xfwsqswu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3mxippfgj.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3yebeukyo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3qserjdtw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3wpdldymc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ckpwzqfa.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3rkrmxwmv.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kmkbhprd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3gffdukln.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3suclhitu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pzrfwriq.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3jsaqpzbb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3lvbzhpkb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kewsnrjo.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3csffwywi.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lbasgmkc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3yjuqhxec.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3mpcgyoqy.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tndyklwr.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ogqehtrs.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ndjasrfi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3qobhkply.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vefbbnvn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jqdbvyhw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwdvgzyq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3heczipdu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3btxhlivw.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3nxjojefy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvqunjxi.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lgyaqsfn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3bwxzfhvq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pmqsjwyz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbaycpcm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fefqcwoi.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bgrnhavn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dkokjkmb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3njkowcaz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3cphasssb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3hxphkukh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3edvbtave.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bfkxpxfo.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dwztccdk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3txtiezxi.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3konndeez.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3bnlumzqi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3tdfkjmce.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3woyaguap.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3bzngihvc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3nymqukqa.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3zzpbghup.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3okxcfwub.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3oqmlwozc.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3nrlqqlsp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3hfuxbtiy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ciamflsv.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3gfoneour.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3dkylxzie.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3zcjsoeju.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3fywpxizx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3kxvkbvfb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3jrzdjzeo.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3blhoevib.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3gzueklql.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3neglpjsb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vbsvgfrk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3qwqinkmo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3gusefksx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3orxoezbm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3djtwudik.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3baxmzqfo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3nvdheqqd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3abkaaqts.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3apdsfvfm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3vszgwdcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hayuibuq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mnwlxrif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhjboxtb.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3uqbcsoha.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3wuxomvrg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3dqbsnrdt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fdoxecns.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yimznkca.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3itossznv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3jcgrucll.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3kegqzbtr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3zlvtzjxa.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3dtngaxeb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3kxoayvtc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ahggnpqa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cfscdmhf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3znekaqen.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3peeouyjh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3duokpgaq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3fimqalqt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3unznjfbr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3nnhbxxjb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3wvxhjsbb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zylbrknw.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vgskjfrk.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wztrpjvk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3etbcybes.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3cswhhvgv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ythjmpay.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3arkqpuna.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3nlzgbece.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xgnoqbkw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3emtjucwb.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3nqnyonok.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3totwkyhw.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lenxhmzk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3bychmbno.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3fjrjxkil.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3itmjreqw.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3wniqukjq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3rdmesrzl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ylbatcdf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wergwbff.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3afzcdfmf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vapizktq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3yjukcegp.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3whqynxog.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3afodyiuk.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ukvlwrnx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3wzlhyexa.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ymsdvrrz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3scuaoiey.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lnnyqbdy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3jygwltcq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3hpyxsllk.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3zbtalsbr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vvjruwjl.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3mhbujfzy.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3xqeofpmf.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vivccvfw.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rwgntkef.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hgxetmjc.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3lxowbwwh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3lnzvstwk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3rptnvuax.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ytibqonc.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3tbpmqcrk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3nznasztu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3mdzrfjml.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3lnwsfcie.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3qurvefxr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3yqlnipnc.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3sitacfjx.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3cwyuzvng.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3vtvxygwo.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3dnlklnej.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3mismlzty.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3xkyxbuiq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3iilrfgdq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3xiobpefn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkypeqzv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3wdhyrupm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3dehfbqvc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3pswwnzks.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3qgbaihxq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3eckapqgj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3vbuwypse.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3reksmojl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ddgqgpay.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3bctmqrjp.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3sxjcxvfb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3ihfibocz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lifmqomz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ehqnqrhg.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3rzbadakx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wzmvtvsn.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3wajejzxh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ejsfvprp.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jotzzlqr.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3itizvglp.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xzirdsjh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3tkxapjde.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3hzeupmpo.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3saxuqapt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3wefjkbwo.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3lfviewed.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3wcjcemkp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3lfcgbmjs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3xctmkjvy.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3vkhtooui.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nrxjzwfv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3qtuboxmj.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3hrbofzpv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nqbnmlav.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3uplatnol.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rruyqguj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3cqqmkunb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3fkdshasb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3rjkfbhom.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3vpnuilrh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3dlglxfkb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3adnzcinb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3yndkypmu.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3gdkssjjv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ucbxbpsz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mhpfjiwu.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3togylpwb.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3apdkjhqi.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3qgraocvl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ospqezgv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3iviabfqu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3sfhwqqhi.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qzrjtxbh.html


<!-- 参考信息 -->