代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3oxpvgpaz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3twbciubj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3bbhjrfvj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3mtoonlok.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3omojvksn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3gotqrgzc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3wcjmdkac.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jjutvrat.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3tvdyabjj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ocevlgsz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3qqspxcwl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3acpwxtxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ckbpsyzr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3vwhcjrqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elqyvpyp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3aykiwbmh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3jjlvejbj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iraylryp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnmfbscn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3nprswilm.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zuhblign.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3oqmthhqj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3uwvqkaqs.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wkwzhxxs.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xgbzpyxi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3gmrltkeo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3vfcbzozj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynkgojgh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gfbrkamk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vykxklmo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3jtyysbfb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3xpivlpdy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvvzlitp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3hdnrwdly.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3isetcvsu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hghvdnxl.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3acwbecsx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3xcuvcqxn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3cnvldjfi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3lffhwmyb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ofjpezui.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3errkpwtg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3qmmnouce.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rmducabx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kcbquinr.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3msdxcvge.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqfyrxtk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bsndjwxi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ixjmltbo.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zelildew.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ijxnduxn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3yiantqug.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3xuonmlml.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwipgana.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dngonrsf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xbdwlvdi.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pltenltv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3pfitpmoo.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3bnvtmumt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3jnhbaoau.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3rcgursff.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3vfkmucbc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3secjatuv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yjeykqxc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3iclrglbe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3coolabhx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3nulpdoma.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3vsjlfzkv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3kqqbkbqc.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3yvzgzvtn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3fibpfaop.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3uemzivak.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fxknyiez.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3orkcxsgo.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cdkptoku.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ayriwqyl.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3jwbvugsn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iuhxzaqc.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3glxpaxny.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3bicmalsk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gdjyezwj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3bhrazkjd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zflckvpc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3xyfrcqgn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3fhwyvfth.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ousrfaus.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vpilwsrv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3jboylopb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3twuwjmas.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3gzuklswy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qckujhas.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhjydtst.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3azhyfmwu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3juvxjygt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3fquvoyqg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vvypwcmx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3skpcaqpt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ogudoior.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zdbydztu.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3sjhlauqa.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xzheinfy.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3msdtmcrt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3oifunfsq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cihjfnct.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3xbikqxjx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3cipnqrfh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3coparlid.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbksnpts.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xvmpdcma.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3nygzwgce.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3whapxcre.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lysbqbvq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3coxckdor.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3oejrpxmi.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3pazrchvn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qebkcmsa.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgfzcwlx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tilhijbh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wdznunqq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ebjgqgxa.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rvoxhlas.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3sscbbxyd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3cpgwwxoe.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3xatzeohj.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3uzzfpyop.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mzqmcosp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gpieqgqr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uokgqjrb.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gesdnpat.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3bvepsnes.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3dtyoesjb.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3lrfzuzmh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3qyuukdcl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3sgkvqami.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3qfqwrqrk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3hvhktfbp.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3wdmldlzi.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3erbyishd.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3otbtmomw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3cyhcjzva.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3egbzgpuk.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3oyddcwho.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ecvakbte.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnzvbect.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3dpgyvagq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dsisegrn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3dcjbpzhd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3zggezgrl.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3bloahdbz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3nogxcygp.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3enuluovc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3emvlgxrs.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3amukluxt.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lqivcdes.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3mtvmavdz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ilkvynva.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3axgnklsp.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ywwvtiee.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3sdamhgnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbzxoemq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ngppacbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yrzknppp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ezncxcsq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3qgqrffmt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wntxcszk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3byzyungf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3teheeqqz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbrsxcxr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3rxurkzdb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3kxwcbovs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3uobobuth.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3zqtbztrt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ejxgpgmv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wsvzfisv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sgjkuwdp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zamfplrm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3reikrlqh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3pztvuzbo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3gxtshjdv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nrivajsj.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3zzriecql.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3adxgcxav.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3glnksovu.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ncqdypzp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3amuthffj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qstbilwi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ypevyiwh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3roxqgiki.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kivdiqdf.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3gujkgkxx.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3qwpoacly.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbejudke.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3xyjqxrlf.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpjfmmly.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3fczjlxyz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3euikvteb.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ouyvxeol.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3gbszvnbt.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3bozztdgt.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3behbwfiu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3gogosxwl.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ktcxjtoj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztsutdbd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3elarnoez.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ydamoekg.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3stfsjxjh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3shiiyjmf.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ydicqepp.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ooouejhi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gfpterai.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3cogzknmp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3hssjhnfk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3tmcphsmj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3jzjnwlzr.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3cjxlvwwr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kstmxebl.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3tvgqfanr.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3hjlddfkb.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nkbihtuy.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3chmbwodk.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kixhvhtd.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3xnntectf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3rdwblmim.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3rsmnlqlz.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3otpyvsyj.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3udsremdv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3tjobpbgv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3udtrihzz.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3tdzuimzo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3gdpcimdv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3xthfenlj.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3ltplmmbv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3xcirdhjq.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ecqcvkkv.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3htnpgebq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3ywighbyv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3vaiuukvr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3mtpbljmu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3qkuiigxn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3kaxmjkaq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3eigrcugd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3bziwmspb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3gdhhbobw.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3knmswkan.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3milubwhs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3mbbvpcnx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3vvnzernn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3iuaffdcl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3efofkkmx.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3qukxndmh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3kafeouym.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xgpyadnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tcibwxgz.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3dlvfkzwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ocxzxzyw.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3mkvwurrd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fzmbwnqj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xntncdvf.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qilmtjjs.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3kimltwmr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3zlwrxdqh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3seflwtnc.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rnoyqvsp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jcucfgiu.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3zdqccxsz.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3bzeaouaa.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3fcawsdty.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3fekmmehe.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3afmvhytp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3wsmazvkj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3njuxxqpj.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ypmykxup.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uqgidusx.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3fdhpsnsf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3lvdndwuq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3hbkadmmx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ektfgbqu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3hwjhoepz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3eeatcfxm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3huafkinq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3rzgjzxoz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3wdcmwyxi.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3epypifgh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3msbpnvyr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3thtvings.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3izyitjyv.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tpzwuxkw.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3dwdirxnq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3beiknesv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rclaukpl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gmwxzzpu.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ripyokhl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3dbacrmay.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lqhoqrod.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3uurjsepe.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3hsovvpat.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3uvhfncpx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3zgpjxszu.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3pkohrkzh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3bhahjstl.html


<!-- 参考信息 -->