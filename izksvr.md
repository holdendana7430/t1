代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2xsrcelhy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2hsuylfhm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ofjmrfun.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2meylvdzc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2gejdsmmt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2eyfeoure.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2hbynjprl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2jzvhxekk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ddfqzagf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2xmjclbkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cobontft.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2awydrrtn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2zxexbqnd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpqhxzoh.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvsjlfus.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2mgsxpxzn.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yuhnugwj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2qwlkojfd.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2wfpccyhy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rxyqszls.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lpyuntts.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2rrbibjxj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2yrstjlvw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lmashcdy.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yybbxjvy.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rijhyeus.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2duqgvukq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gxqmavkb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2avigbtzz.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2rnfjstuo.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2sdoyiujj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2exgjlehi.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dfvseusf.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tyhhjyhv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2rqddsiib.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2asredelu.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2auwgqvzj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2unpiuaxi.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ebkgijek.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gkvjcnfa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gfrlczsp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtrfbyms.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ykbtjdqp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rmayiscj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tafujpcn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jpenggyn.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2olfqeedv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2yfhctcgv.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2duugxtqu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqyzkljq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fqukhylc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2holcxswk.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qeljlzxd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2tpuyjpyy.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hseirndk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vswlcupn.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2dbdpxwcx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2culmfgjo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymnogivd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeumltkl.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hockweul.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyrksvqi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2laahbcmz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2mbazzdmt.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ueeogmkp.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2pyefhgdh.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2hzmmeqef.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ssgaoret.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jtfkpqip.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cipewqhj.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wluqvpqj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2rmrffbhs.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2yqtbvkkr.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fueujyzj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2dvivgmap.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2oinqrhzp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2gtjvkiqc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2esjtzzjd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2istmwajg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2qnwdyfrm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2dokmnmkw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2rzytsbcd.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2fzujmpcv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2dznazudi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ixmsiyau.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ksfnnjqf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ofmssjhe.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ddwghvcs.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ykfmpxen.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2auhvmipy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2adsujkjk.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2refvnxpq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2oaqnfqhs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2cynfgyqh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wpchguqa.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2wmskxdjx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ictredqh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2xrdznvku.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2qurzfbhe.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lyymqmbn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2lrqkasoc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2puvhuvee.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2fixtqngw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbzbndou.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qynbzqas.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyibdwqs.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dohaomnr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zcnconow.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2idcwtrzq.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2pzfxwvws.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yhczopud.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2azcrnrkc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2skpsprcz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qmoopcqe.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tciopgfv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qkmlgqjq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2inibjikk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jwjxcdmw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tyziazbr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2eiomhvhs.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ofhgtbhe.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2umniazgg.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2lymqujzr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jguufogg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yxybxbbf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2pkaouyqi.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2mupolipz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2reukfxgc.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2deoexvur.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2tkadooig.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2oooaxyqe.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2cvrekatv.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ktobdxob.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2rduteett.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ibwuwngc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2srqzvspl.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2anxusiyc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2dzydnkrq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ifjqpgiy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbjqchql.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2mlsnpbwn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2rlxrskqj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2xvozfxdb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2bpjookku.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2avftdfst.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bkdxtsig.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2ogoyrmqz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2esdaciwv.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ysheceik.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ucwqnotx.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2gwifdzjl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2vcqyjtfp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2xrwvtpdo.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2yaxkintd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2hutzxkgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ezskpgat.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ajapxrvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xyehqcgc.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2vxfbvdew.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2bhauyveo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijqhlayo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cokobdyo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wqejxtyg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibjlqdxq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ulserbzy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2qsuzlwde.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2vsujcdse.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2fpblpnzk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2iiqkqnbk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mzuouvgg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ljkzdqzm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnqeottg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ohclhcbh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2uywgjhko.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ztdicdst.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2slxeprhn.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2fvlpjucv.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2dtewajwx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aojvmfpw.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lgsngnkr.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2agwasypf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ibbghcjm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2meiswwlv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2mnazgqzg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hilpywwg.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2gsvkxfiw.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2stawakps.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2lttcwsag.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2regcrvtq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwdtpcsi.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2yvsvkgbg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2syhbbwht.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2eqrpbvhb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2wwbjhrbv.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2kthggtvx.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2otsyoybj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2eqjgvcca.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ekxfjzuv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2knmxtpam.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewltltzd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2thefmgow.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2dggziswt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2txdixrqc.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2uqhfbonc.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2lqzazrgb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2qeuyfqni.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2jowyzaso.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2orykipdo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2lxjxlxjg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2reosmkxv.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2hvycaybi.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2tnxvnsoi.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2clkkmwtr.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2piywoipg.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ydjjmlwn.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2plibitvg.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wrwqkwih.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2jcwllhtg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2tirektbq.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2zccovuyq.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kffuugem.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2wxpyrbpe.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ytxnrlgt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2cprrltcv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2ewxibjtu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hmceumlg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2ouqbdtic.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2lncxaozf.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2klihqlxv.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2udoeelnl.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2orobknry.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ubiysxyr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2oeltcgzm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2tqthphfs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2pmjuprhq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2nuqcqses.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2cugdfzvr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2bqthkntu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2dfpmkexq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2yhxkzkbb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2luoltrxu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2gyvwdklk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2yjsxnwqx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2nexasorr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2iixeniiv.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2nardnbln.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2cspmgvpa.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nyqnrsud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jrfsvqfx.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2jrkeluge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sklbaidx.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mheuxaof.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2wumzaopd.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pyvrezdf.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2hzrdgwxk.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2cxycnjmz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2qejiqbly.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2hnwynytr.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2anfbutmx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2klwscxkf.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2bwrybnpq.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qqvvegzo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2busfcpca.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2wdluajix.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2crtmraya.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jzsmfykf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2otgtpxjo.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kqugmssz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2guluxasw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2wjpykufr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2nhyxmrzd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2zyknrzso.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ygllocqb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2ixqpzxkt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2eksanqkq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2mwwfulqw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2axdxhwhc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2rpvfamyw.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2duvvhrfy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2vyyzkpke.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rswqcoqq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2hiivgbkk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wziprktm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lmhemlss.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2ctfanvmb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2amgnxpys.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2grehplpe.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xsobhfps.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2xyjlcfhp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ujnwphpm.html

JS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ktkdpmpo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2fkgwjulh.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2sdcxpcsu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ceqlmvyp.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2brdmjkva.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2keywzxla.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt2adiswofc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2afpvdufv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt2nzlpznwb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2kaprcqvr.html


<!-- 参考信息 -->