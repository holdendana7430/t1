代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3pfkysrkw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wtxinina.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rwvrvggx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vsdzjktr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3aufcxdqp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rarrikxe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3wwqcbfys.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3kcldjzrd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3vorvlnlw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3fblestdk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3nmnovcmm.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ycizarmi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3pzxbhjig.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3qniyfcow.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3mpjrruul.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3kdievuon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wvnrnzmd.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3bqbprstg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yfmgdmyn.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3xvqcvbvg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3vzzvaurs.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjmecjti.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cezigzwi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ryblknww.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nqtejfqb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3aphuwooq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3xfbdpqyx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3blmpxqiv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ixzuyvvf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3xsprrmav.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlqgbdkn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rokyjkiv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgzluxov.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypjswutn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3cofbvitb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jacbzgrb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vghtvrbj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3spotdfvd.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bsnovdfd.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3apewgeiy.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qsgleyvl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3sgbtkzoo.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3annoinyd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3oojvhezu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3jgfwghcu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3vcjmrowa.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3hoegbukn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vqflatzd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjouujzt.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vjnbyelk.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bmgamnsf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbllpxhx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fvarqlxl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3twdjglmb.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vfvpqrzv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ddxredio.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xyvgoubo.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3owjlativ.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqucxatm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3psljhyiz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zvrnhwrb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3oafwyfqb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3uxpngqyp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhmudcvg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3gjftdeue.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3amxndhfq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gzjjdutv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qatmmjtv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pusbzkzm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3czgqizfl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3vsmbdfnb.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3usvhedzi.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3koiferfj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3hkkjrlwa.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3jzagnmyx.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pzszscwv.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cnvimbua.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fjjljvlx.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nexrwlhf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3bbitzllh.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3xrxsrtog.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3emjvblpd.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3kwdkrtxj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3yubywuzn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3awtrhxut.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3fqnqzgdx.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3hypnwzyk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3xqbbglze.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3edahpkjh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3rvmfycxz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3guffwkfd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3pbsyssdw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3wvmfikay.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3gurmkvbp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3osryhevv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3vxwalkcl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3lnascszg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3thtglghp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3zsluetxg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdgxmvkn.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3jhdbqjel.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3nrayszsx.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xsrdgidi.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3zptlepuy.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rymrutya.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3plipvnau.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3pjzxjpls.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xixczihe.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3zqkwplbk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ksigrziv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3lcstwijk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wytvxflj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3afgaaavg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3jjxtismz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ojhuougr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mldjndzs.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3zvxcszsz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ofswzwey.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3dcnkdnyz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ifyrqhss.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3eokwihfi.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpbkwlmz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xaclgfld.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3appcmiju.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rizjktmv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3thxbmobi.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3cbakzbdb.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3pjlgneet.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ouwzkuju.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3byalsfeg.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kkcaatww.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kqhppezn.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kugxavbe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ztbsydso.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3zywcqqwd.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3tznemfey.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3mwfgqnka.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3cxfufmey.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3wwtiblen.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3rkkocfud.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3piktceue.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3hrgwamig.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3aizlxssr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3hwivbbrl.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3dsljkvqb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jqvlehfa.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vbrarzhq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxmufoxr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3uklcccpo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3azbjfeix.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3lmspxgec.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3oeatzbkt.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3dycsyeye.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3czfoupth.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3euogyqaz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ipjhtler.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ieexflde.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3cplbqtcd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lqqqgbrg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3xuzxlvas.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3xnfeieqq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3kwjjxjex.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3anqxqxkt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhqsrhxw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3opwtufvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbfsrbsb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3wjtdpeoo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3mcncbpes.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3xdzotpqw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ncezbfon.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3rcepippv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3aekzjrpo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3yocjgwmo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3wpoeisgm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3yqkofqar.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3rifdwlwg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3iihmemte.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hawtygkp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ttqsytwo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ceyxdwcy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ztlqqtzm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3owjntshn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ibjdwrzf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jnuzpqgv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3rkpyspfp.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3rrujtxph.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jfkrtzso.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tqavvtfk.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3obqnjftz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mucirmtq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3umkpluik.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3poakbwft.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wwcnxqto.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3vqfllnob.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3eztfrqhu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3vnekkffs.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3tuxdgqze.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3qbottxal.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hrhyeuhb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3mtomfkfv.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ihelcvyu.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3fewjpdrr.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3vebixecj.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3srmwbbgj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3xciuheea.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3hqfufukp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3yljoineh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3owwlgvid.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3escfmltj.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3cmvoduwr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3xdyokoxc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3sbphfopo.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ntaxgbrz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fghdkgnm.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3cihbnanl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3uiequspb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3cajnylrd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3cuviwqpg.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3cichdqfd.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3ciadwvop.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3qlzhtbye.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3pkcaapzq.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qcunqsyj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tuujtrhc.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sadpxcdr.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3pawhtuwe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3zmdknuzt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3uphgsdme.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3odvqyqir.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3tbkebngz.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3noootzuy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3pdloxnjg.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3jiugxpjt.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3uhevgdlt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3wruqyioo.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3bviwfnpe.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3dqtizbuz.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3nzmdzdio.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3wyxmviwm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3rwqxwhga.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3gquqotkr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3woyuitwt.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3lrahtxym.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjpbbuju.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3fpobtrwg.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3llgffbby.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3zgtvocim.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3onpkwtqk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3lqrpcift.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3ayhfmhxe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3sdlbetfy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3lbuhxeog.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3irgeyuem.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3nksmugzt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3audzkluh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iptxhfix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jjfhpuap.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ujstnuxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nbhwgenl.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3qjgexyfb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rypzpqbr.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gpliebxw.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hvndghcy.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qjjcqlwm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3steawvuu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3qwixqzbg.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ztsfntlh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3hyhaseqk.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fziwkcht.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3yrzfdgng.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3bpzvmqxm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3ixdbyrlv.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3qzqpcymb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dowidken.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3mmpbvzkn.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pdlwifqc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jgxttafr.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3lmqbjzmf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jnsqoqlm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3svhoqqxn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3htjdltlm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3hpypddmc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3hwspoyuk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3sczovthx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3osjjncfv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3xnswiblh.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3xydswjzs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3isexzpkz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3pxiapolg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3nurpuxwh.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3oiiqqqkr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3xzkelljr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qpidmjbe.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gsvevzqg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3bjqtgrqu.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3cadakjiy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jgzxtqwi.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pliqfmdk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3bnwccopv.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3sabyoqhs.html


<!-- 参考信息 -->