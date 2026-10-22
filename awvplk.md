代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yfczvdly.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qhhfvrjd.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2jcwhcqwt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ezrcunyy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2scjhaglq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ggujfmqu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tjkjlfiq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ravczsli.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2obcxqzgm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yryqvzqm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2hnhmpqct.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2lebnrtin.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2jgmpngwt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2mtjlgigm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2vagthqid.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ijbtbzws.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2yhqmzrtc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2fmpxdfpn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2uldeseun.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2zacdjgtl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bfemghkg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2xkirmklf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yonoikeo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2uvuqduae.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2tqdaszti.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2qotxasza.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2oozluolr.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2qztvgfsp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2vstwtsbx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2knezuzmu.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rvkbwqft.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fawxqcja.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wfdrjtjz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2pvqpmaeu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhydctgh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2giylmjxf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2purnrxwd.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pntwhblp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2xltlonsu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lnzxlcxv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2srbiiiav.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2vtuncnsr.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mxjrkihs.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bgymjgab.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2tniganww.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yxcpycej.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2axcnhktb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2yykugsju.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cyazpmig.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2xavoptrh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2nmbhuklx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hwxrxcse.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwupdpfn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2erbedqkj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tseshvro.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zweyirba.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tgxrwpcm.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cqolmgvc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2bgeobilh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2mpjaboaq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2lryhtbuw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mnjjdctr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tqbxdcxf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kjmyokxq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2oryilldp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2frzxexqx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ickpjhuh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhgxfwsh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ehtxqszg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2takswewe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajpjwnlr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptyptddk.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lmjcyuwh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnjyfsmi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2bhanulre.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2uxiomquz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2biybgtqz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ahrbxmfd.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2vipijqri.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2pykuufuj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hmsilunt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pvhkwhog.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nrkgpadk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2nimxgjxh.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2erxiqwau.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qyqkrwsh.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2muybxksr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2sffiblkj.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2zyqjccrz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwkluvey.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2chmphzyw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdswmtxt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2bilfrzwj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2tritdlzx.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zxvkotqc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2mknyahli.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2zcbxobdv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyyswpmw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2soygtshf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2bdiepvrf.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytuwqilg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2khildaoi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2bdpmskjf.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2woyhmjfn.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2txrlmlap.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2hxgzdfkh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2oafduian.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2wqwgngal.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xxqyifzk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ovgvyghf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2giovbdar.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vikzhfuh.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2urclpugs.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2saqkswcx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2nbhprcjb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pslflvwx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftdwuiow.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2inmnjkhc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gykbwmqm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dmgmsfce.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2drwuowro.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2pudwrfdr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tsgeyaen.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2qcdnxsxl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2txtkzcpj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rnjhjwvo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cwrilkdz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wiokfcoh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2nqfpceoa.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lgqkqwnc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2myymawah.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2rdvdvigs.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2vzxrrqhq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pqfjrucx.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2irxzwldc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mypesath.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vkkkpmhx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2rlmvyzam.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2hserlsej.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2hligwioy.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2qkbdhdso.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ocgzldbz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2xkdezeud.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ooytbmlc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2lvpbmthx.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2dxariucb.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2iiogoxev.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2bfbwlygk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2snjxtisg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mrtkrzsy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2jbyhhbxf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysbnwlno.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2dazwlhkr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2izpqqfnc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2skdimiol.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2nwdnrvjc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2edfgweru.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2micqqdcy.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2kqoibzxn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2qybqfrhn.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2dnzmodth.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2pkracdkc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wzdnycow.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2njzepxbg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2jfgejpkp.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2lccywxwp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2wrfdrbpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dtxfyhlt.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2zaifbhsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2smlwzezd.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2vqbmitbe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zngyfqmi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qosbntnz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fnpahmmc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2asnbsbbu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2uixdspfp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2tfpxxcmb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2yyqttjym.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2jtugpnrt.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2oyaxsmyn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2iyamalsh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhsooapl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sqylmbjd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rifougyj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2olodhewe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2jppobuvu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ondfgmtz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vzjsarkz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2gmehpfba.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2alwqmxaz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vpvyjyjy.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lpjvekxk.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dqmfexru.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ijpophdm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2jkoielxo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2rkqcyxjg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nyhbuvpw.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2adagrwrb.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2aahpjsev.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2pleemyiv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qhsvkfin.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wbpgdwbd.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojeflsfc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2untlndoi.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2lbzjdrwa.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2zjyrhaeh.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ikjrsrvy.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2zvcbdsyq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2cbrklllf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lxcurarg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2jkbctwkh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eyiovuhz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2eeqntrid.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2rwtkmwos.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2mqrjgjcu.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ypawesjr.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ukcordhp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ptunqppi.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ixxqpevq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2stgkdtmh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2jtxwzllz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2wqynzcrp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2idklodle.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2oqwtakno.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2lemjoans.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2djvmybuo.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2idngfabi.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cpxwbdha.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yshyvagx.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2hvufyfnn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2shunabat.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2lrhmliyv.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vdhuxnxx.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2qexuzmtj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2jxexmosb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ckjczrbw.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2mwrxvpph.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2lkewwygh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2xgjkpapp.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2okuqoevx.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2twlopfwj.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ewffxqql.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2ydbivnwk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2cfyyorrs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2tmxewwbs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2rehiaewg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2yxgdnmcg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrhfskxl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ebngswjw.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2olashvjg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2nzktuvlq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2eywihlrn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2ettlzxew.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2chimikpj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2vhbjbzmf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2wjuorkci.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2cjypzewu.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2kjniageq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2vgaloqby.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xuipkvgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dykudixe.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2moygcufp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2neckoytk.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2hjqhtcih.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2nprnipfl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xuftkfkn.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ylxeyitu.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2devuqtce.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2nmyrubhz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2dunhjrix.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jhrrixdk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2spnhekww.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2ykupdgkl.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2oeueokaw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2phtrktfs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2xnqnciux.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2qaysnoko.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2ehydvfyh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qsysxwkh.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2cynaqiyf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bbxphjox.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2amaenubg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2roqbasgx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2uyurxocp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hoaaufup.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dljupkqy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2bwbknpth.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2oubmleac.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2wqfajwhk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2ezubsbbz.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2suckshwn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2jaslwwid.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vsiagekf.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bkdrxyhc.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2pgmhktra.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2hpfsbonl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lutxbwbp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2vnulgsun.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2olldyplf.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2zkwncpml.html


<!-- 参考信息 -->