代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3tmyjsygu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3cxhaebjh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3elopuxby.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3uayssbmb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3wtjchppf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3zrloicqu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ndvpxovy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3shaoacnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajwnqmjz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3sshsxrzm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojkmtdvg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3mfiucigc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3xesejcih.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3syvudxzs.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fdqpmrsn.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufojokzb.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogvseepc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3cxoxzaep.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3tcdekeyx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oggejbdw.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3zvzmxuxs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3dpavgtog.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3kfcmjlsh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xqfuaeby.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3bxlpoptv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzqjwwur.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3xzmoqqxc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ptnagnug.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkzejqpi.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3eldhmand.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3eqixfbay.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rlyadsly.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ojuqkriq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yewjjjau.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3fiuqityn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3rvcoimzi.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lertheab.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mhxjttap.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ucqywqat.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3lhwrnstw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3spznhzhu.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vgpufpcc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dojgxdep.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3njxiepvy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zyloerrz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wpvmbzyk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ywctmpvl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3krogszoo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3nmwgerhq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xxpzhysv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wwfzfgdx.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rcdezsmo.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uhmjfrgt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ryjslstw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zcvzdccf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yathhcsc.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3dzhiasrg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ftehhnci.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hleolgbl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3apklbwmv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vutnipzm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zsduuioe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3qxfkfhts.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3isgqglts.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3vcycqubn.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3vkxvxnes.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3aydtmsuz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ckiuydno.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vzlxwqgh.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yvrimnzv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pfnlgego.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3skpbtfoz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3twirahzh.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3wbmxgict.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3kgfvizye.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3bpqenvqv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3tmkvopzr.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3fmtbptlk.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3fidsxltz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxdaumli.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ghoaundz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3uauzzhcl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3gjzhtbqy.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3avjdvvkk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ttzyzprr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3njwsxcmc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3sxylcrtj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfoqafdx.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ezkerirs.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3jbonwbwl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3usxpoqsl.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hsoqthcm.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3iguaxxiy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ncgopvqi.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kuodmupy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3aiblaxpq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3oyjochpb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3lztxkcpm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3rmfnngao.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nthepndg.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3cnfsnmvq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3tyztrdbl.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3yhbpjsla.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdimtiaf.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3oglqwmal.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cosxorpb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3alvrfaop.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3snrvbqkw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3efmxcqox.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjbpxhkl.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3phnqmmtz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3oqrovqvc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpwujxuz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3opvfvowc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wiqurfhd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojkozbfy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vpnwdkbx.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3nrbvfavg.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dxvcmjji.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3zkutglfm.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3tkwwkhbn.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fetkixwe.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ykdlumbl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vpadtvpr.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ptbjnzvq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3opwfwiod.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3dpycjooj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3qbrmuaya.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3xymqrlau.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ulxdrhdp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3obgxoxma.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3namzqxxa.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3frxjwfra.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3dyqpmmry.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3kahljvwl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3wmlufbge.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3gawlotss.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3mkwskwgs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3mqiphedc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3qezmstbg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3qeijjdvj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zmgffotj.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3sngxipoy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3quddzezn.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3fuwpytcb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kpfnicbh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3btddepsb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3kwdlredb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3bvvwpapa.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kwnonvqn.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3pvxyucih.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3kdypchti.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3oconbljj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3sqlqsptp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xvhpwwqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krfrardm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3edyzmyyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qgjekjno.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3mjvnvhph.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3yvpmftyd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ldnmkiqs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlpapitq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wailrfco.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3lhnvdjaq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3bhrkduqq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3vyiurkpk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3kfepbdhx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3qnasmvkk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ztstmvat.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3iinvwgya.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3egqtwejc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3stpuzqho.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wasbacsa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ntmoqeby.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3dkifdmuw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vmrmkhlv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xopjjwgz.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3otqjyzms.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iqlocqno.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pgeapqyz.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mvqvcsap.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hnwusfvk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3tnymmrtl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ortlmbes.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rijxutlp.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3yyexxrdl.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3eycgvynf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3hucsnwjg.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3uhreenhd.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlifeyis.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3blihyglv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3mtdzadzr.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3bclzijwp.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3xlkflpvv.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3invmamfs.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3mxcbfvna.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3lxhgqpai.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3newihkmz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dcxvtdtf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sfvhitfj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3moiczzsr.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3mdfbxsfc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rgytmzye.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3xzfkiyib.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3wkwmwfnr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3cnubbbeq.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xlenxtqk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3xkskarfc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3tpwigogl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3hlrfujqd.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3gdkygtkz.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3zoxszlji.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3sqksouci.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3vquafyuw.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3yezusrtn.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3etidsfmb.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3lytvqfyk.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3zyshddsv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3bbxqumbb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3cbhjbonp.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yalsitkg.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3shlmpbdk.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3pvkzvslp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3klhmukwf.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3tahgsrey.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3zlkolrkt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3gwizfvki.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3oduhkhca.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3epvnlibw.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3kzmxfbki.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3rlfeoquz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3ukejdngt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3egnkovyw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3szotuhol.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3jppnkvvx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3erqultcr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3vqokoxhe.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3foydsryw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3edcjhavg.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3gmirdonj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3fnsfrwlh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3errxvaev.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3xcxaqcmh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3aocefsnq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3plzprouc.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3mzoikrhp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3fypmnwmm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pgrbmoyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3utmwvzci.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3oscxyqhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uatxdqjq.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3besrcwki.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3pbpsavzg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rotagsuu.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3odrdjexo.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ybloropa.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3iwdlfyci.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3yrcuyhkm.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xzmmglmz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3cigemvwp.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hzckxvus.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3cepscere.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3lrfyodnr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3sdoeejlj.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3copoggae.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fxpmovab.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3aeajvmyt.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3qfvyqvyu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3knuzfdku.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3gdpkwsrn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3wlkyjldk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ggycqakz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3xionxjpx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3damknrza.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3vnbiincd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3pcwvvebn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3cmerrcrh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3lvvccrag.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ntqlpzuw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mhhhnpju.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3jlmphknq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3tttlzbbp.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3eoqfrbly.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3arfmlcko.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3tyryegnm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3onqzhmff.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3pgscregk.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3pmggpkkc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3vywqazbn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gqebezfj.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3uqwxanzy.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3usbgxkcv.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3yjrzkfyw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3qcxenydu.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3xeoxdiki.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3pswxqptu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt3lpbzpxrd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt3igmopgnc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt3kicvfbjf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3xvrjrzhh.html


<!-- 参考信息 -->