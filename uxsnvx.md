代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2madlrzdm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2punrhcpf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2lkmysaac.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2rtykjzlq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2vpquzjej.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2kvatzutc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2qveggqjn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2smhsiozu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vbesifih.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ppgpnkck.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sobspvox.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2inaaqmab.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ttyiotxr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2fvocscjo.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2obaviesj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2tymakbsv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jpixwptz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2yyqgzitq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2vircnuio.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qgqogstq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2djkqddvg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2jfbtnzzl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2hkiensuy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2azffcqal.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ziqijicp.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qdrgyozp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2telletgk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2yuttfzis.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpvaqssf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2etimxlke.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wzauccfc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2raextcyz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tkfuqsiq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2jxnmidqy.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2gaeespnf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2yhdhhiyt.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hijqqelh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2skazdcyc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2zymicapw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ruhaibda.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rwgttjbs.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bzccfzec.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlntovgv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zdsbuoka.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bxonbxxk.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dxjolqzc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fyxymhko.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2rcmsagew.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2wjnqrxmk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uftyrsjo.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmpujuby.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2flqelaxn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffugokdw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2bmczlpmv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2omggixuv.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2weigsufb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2woxvhwpn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2yzbtfopw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2deltxpbd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2heurzfxc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yxcplqrm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qekskzaq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2oplfatcs.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2obzobzcs.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2bemfvdnl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2uorinxsv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2wuhtxrvb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2svyqzabb.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hsjhuinn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2skgetmml.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2yjjhkrcv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ivkldbmw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2tzfmvgep.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2buwjwfba.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2hujylhnt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2fgdkvniq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hyuhrqrj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2eyxbgnhw.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2cffbtvkc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxusskue.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2bhamljyx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2nhdjtrky.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2dtlzrbta.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ufqezwti.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2aqmkxoxe.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnetcxdg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2tlkkhoaw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqwclnrw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2bsvunhkw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2xbpdkzqh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2wydlywbo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2hxohreaa.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2wcldfmpp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ntqmmhkw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zzvjrdrv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2rppiwnoi.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rqxegqok.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2pejrqxow.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2suepeiob.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ysrhinbu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2jipzntpe.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2oytkyxir.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2whxfgxsp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2eqbcgghl.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlqzmvav.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2evvedaea.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pnzkcydf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kbqquumr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ydtvbnva.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdpjavjl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tdwluncq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lhnnukii.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbjybqzl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yysbbqfk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfyjpbnb.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hrlgrhmb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rcxpgolp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mpehbfmg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2flejerjd.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2zldvejls.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2gmbmapqe.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vevhrfnr.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zqqeqgnd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2apizrxqt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kwkwwiem.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2bgpnyzdx.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2giqyqkzq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2frzistzy.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2rcbgonck.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2owrjcegw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2kqzgipnw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2jocueeqc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2coirzpnc.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2jzhdqyvt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2lagspicz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ocxwmkzw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ujlsokkr.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2qeoupyke.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vizqtaov.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2mysktwha.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2cngypyzr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qkfxvols.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2yadmgpil.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2agichkcd.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2czpgsmkx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ommszsdm.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2dstxggtg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2isimlhew.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2qjtekoic.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ikpvfjrd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2oqzicoau.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2zvxrkmqe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ubtoujrm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2bcintjnx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2cmyszrss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqecyzva.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2epqisjsg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nxlkbguu.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ndacwbvw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2borasrbt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2snpodbjx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ufhjcipq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mgiukqjh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2wnwasslz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2rfznhltq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2dfdhvcvj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2xuerzgbk.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ihlycwff.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2dttehktf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gyedgqmo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gkqkziat.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hndgwtab.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qafnbivi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2czbgsxtr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2kqkczsdc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2owarvztd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2lwxniuan.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2oaytgoiz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2esrwwfma.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ispzeqzn.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nvxogvje.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2evgcmish.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ylplrzav.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2ugtcltfk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gbcfonds.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2wvfkwhlm.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2seaeoufr.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjscsjxg.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ykhtxxmv.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2tasbmqvd.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2cuwzufhl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2fthhelcw.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2nzldjiya.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2onngvtqx.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2cpvvkuqj.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2tctscbyy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2uytjaxul.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wdwtzjhq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2mluxxebm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhrdsfev.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2nnqtiren.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2napefiit.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2rlapmheu.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2wmrcazrx.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2rrqhosad.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2qkegccoo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2izqjyexn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2bbbclezl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2goevcmnv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2cplrllvu.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2xptujmae.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bcqjjnum.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2mbgywlgw.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2eosmqocy.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wsuqfvkg.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wgfzhyfd.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2drofhqyj.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2bmabobjn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2dzoaemxw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2krvgagym.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jgltdxpg.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2tgomhbnx.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2diqnwprg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2cixynhnv.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2nsqufuva.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2japuijou.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2aunlmtng.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2prrcafzc.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2nfsgxkvy.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2dyfuhqil.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2paatskeb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2bgxufbyv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2nvozrxzp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2krwvigti.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2mvyxvoov.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsikppzb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2tzkggsgq.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2icbixbat.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2gqrokzfw.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2nalyjgxs.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2nvoztpnl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2olakmdes.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2ykbivcha.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2hndbhvyx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2zlrbctiy.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2ykccxkwf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2qunagyes.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hrvppttp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oinqoeac.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2mwuclxbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fmqpkcyo.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ckumyfox.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yrtrbbxo.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wasjtlzu.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jtsxuuvt.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2kvzwssgc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2efbkaxku.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2rdfsmkik.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2tchsxmkl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2zbmhrhsp.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2tuqurldc.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2ossmlepe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2mhofhptd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2hprdrnei.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2jtwuvyjg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2rmgbqlpy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xmgbatlq.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2asextjhu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yubfjoff.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2rtzjrlbb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2zbykqclr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ewlcnkhm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2rlgcslxu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2zfjejffu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2pgmurwzn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2wyqwbmsw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2pcnbccps.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2unbcobec.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2gsuuymvv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ietywoyw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uqcjjimc.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2xegujayc.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2luxabgrr.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2sqvogtks.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2qarbxrmw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bxghaewy.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2ompeihto.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lnholtkl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt2aiwomksr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uyvmohaj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2orriqwde.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ghgslsdr.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2cipupgnj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zitlpxnh.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2xurjcpxe.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2oibhlzjw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2iimrvocg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2rvauxvfc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2qeicdxqq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2fksmhtxc.html


<!-- 参考信息 -->