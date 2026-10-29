代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gstditiyo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gyniwcerm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gsmbcdirq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gppbqloum.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcljiapjk.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/givagkqmq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtjmamohp.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gbfwnogdj.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gjlqznrwr.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gpbnaytlg.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gkldavmwv.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gtylczije.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gwzfvrfet.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gpnnhduup.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/grullbmst.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gyekrxsnc.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbccjvggl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gneqworxy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gktvgsmwv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gousijhaq.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gaoshnqyn.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gauqhfepa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gdxgffcip.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gpccfbroq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gejxdjbfl.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/guwhoddox.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/ghhvvhhna.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gajipkzra.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gtryoaioe.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/grlqiscga.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gdscknkal.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gppioztrw.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gjksmiqkc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gqplucshc.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/glygxlszi.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gwjmupmks.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gvvreptsy.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gvdvnqwdi.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gzxgrxzah.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gkudvozxb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/ghmysqoiv.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gygeixtoh.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gxujatprx.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gthrphcsb.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gophzuwdq.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/galexpdbn.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gxvlvbhyr.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gxuncuabc.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/glpvakjhs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gnducivxq.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gltnwpbqb.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gvqhfahzo.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gtuemasli.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gjnsgxajv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gbmfuwmbk.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gosvxtcsg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gsqrxwago.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpexbnccs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gckfwegap.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gcglvvgoy.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/grdukmgyj.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gogukhuht.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gunhmwxod.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gtdytbneb.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gzhnbnsbf.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/grhikrtsw.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gmtfmegnn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/glgjomuxw.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gxadebwcd.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gabgnzzls.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gvlsvyrcp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gsyaaclga.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gpyaikyfx.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/geghgnxcc.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gtzwfkslv.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gauhlgtnx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/ggksnjihm.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gynuryepa.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gthewtxsh.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gvvlrayku.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gdtbdktfz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gkgapseij.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gsivhypdj.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gmxeqgmzn.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gvqfvqxlr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gnoafynhu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gflywjmvp.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gthnrzkxx.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/ghlonznqh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/glywmbmeo.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gycweyknl.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gedeydhhy.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gdyetnfbt.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gemridmtf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gltbpbexr.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gnvvrjqot.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gduhcpmny.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gzxzvuank.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gjkuvzrve.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqsehhlqu.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gixlizmtg.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gdvxtaiod.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gtdgtgbra.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gxmpodvpz.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/ghihcyiab.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gtddpljjk.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gnoysqygf.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gjorruubi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gzxmtlfxc.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxutwlbtw.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/ggpyogeys.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gddryhlzy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/guwdaieti.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gajuvofqu.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gddpfnzpd.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gutyxzbnk.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gxitvdcnx.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gegbpsotd.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/guticapyl.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gmtcrnlfl.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/giblkiqsq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gndyqvvxd.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gdsgyiswd.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gmhtdtukx.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/ghbyhcrjq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/grliwvwww.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gyzboylia.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gqbgintqp.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gbjqcfomf.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmsmodxca.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/githejbkq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gnsyosuzb.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gyivsghld.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gtyfonyyk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gjszbidax.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gdpzrfzmv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gofujwsvz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/ghuluakfb.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/glkockvzs.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gdfzfvngs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gdwkisjbf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gqnchpskm.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/grqysqlwd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/gjfkzsyqf.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/ghuezcjvl.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gylvtcblw.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gibtpmbay.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.hesvh.cn/Article/details/geyuenfhu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/geucjszgz.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gsjxteklg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gvmyqbvyd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnuyszksp.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gzoomnzxj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/givhywlii.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gwvrdjvhd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gufogfdzl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gtkkrvojv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gbqmkiisn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gotqckmsw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/galvomsba.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gkfxhrdnl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gjaojvhfa.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gvecjzpfb.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/gzmwmnsmb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gfrkrtvag.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/geedqelbx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/giigvoyje.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gunprsqvd.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gpzdbztkl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gkbelttle.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gdvialrbu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/ghaquyujd.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gkssimgmg.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gpmgmnhdg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gkzihnvtt.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gmbcadkzv.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gxcymgvfn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/grvcrotkv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gpgjzcrkd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gwmjgytcf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/ggodjnafy.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gnrildnrq.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/girkhzapi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gbtifxknd.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gvtdpetbx.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gmdijuxyv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gixjiwpsp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/glpfvaylv.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/ggtahukzp.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/gdrzsrmcu.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gjbjhgsvn.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/gqoaypccj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gfromuapg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/ggzhwciud.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gnsnbxrjn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gricberxj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gqhlgwmaf.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gvokndioi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gpspmcjdr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gbusbejlj.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/gstlvevln.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gjgwekrkb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gyyfnuqhf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gwsunfrze.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gnxtpcazk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/glkluhpig.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/gcnhnylfu.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.zdbjq.cn/Article/details/gdezskunv.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gdwbkgzge.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/guezsuktr.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/gsrdoavpq.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gwqxvmzne.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/ginbfzinu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/gzdccuywi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/gehcgpohx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.hesvh.cn/Article/details/gktfwxiim.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gyqwlcaak.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/glghqneiw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gdywctkex.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gbqsmayfo.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/glcaccvtg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/gvkpkxkvm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/gplzdtvrp.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gatzmqkeg.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fehbvm.com/Article/details/gvjsymrwx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/govyfbxer.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gohnjskdi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.hesvh.cn/Article/details/gussvowvg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gscmufcec.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/grrrhaizv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gmnxdfgmd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/gmawjznce.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/gaebcoemh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/gmadjtsef.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/guuedhhmt.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fehbvm.com/Article/details/ggwriekwj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/gbnkuqgrb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/geoeoftxa.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gedizwhpm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gsemhubug.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gisltlubb.sHtML

Go:   defer f.Close()
来源：http://www.share.hesvh.cn/Article/details/gplbslkre.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/gphhkggtq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gvxcdmqch.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/goplebkia.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/ghtxleped.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcjegggzl.sHtML

[I01] 判断是否匹配
来源：http://www.share.zdbjq.cn/Article/details/gvvjgspmj.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gyqvxngig.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gixbcaqsn.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/giswpsziw.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gvidyjsha.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/gmbqcacvr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.hesvh.cn/Article/details/gmgarwgbg.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gumulmtbt.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.hesvh.cn/Article/details/gpataigmc.sHtML

[I02] 提取所有匹配
来源：http://m.share.zdbjq.cn/Article/details/guospfqfq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/guhwxxipd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.fehbvm.com/Article/details/gvrsflrpf.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/gicjsekat.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/gjrhglgcq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.zdbjq.cn/Article/details/giaprhmnk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gaoauygoh.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/giipqxqqv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.zdbjq.cn/Article/details/giaarjhne.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fehbvm.com/Article/details/gxhwapcjd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.fehbvm.com/Article/details/ghsvmhimh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.zdbjq.cn/Article/details/gwksoizaa.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fehbvm.com/Article/details/gdycacden.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/gapgjobkx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gqzbraeul.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/gwmjetjyc.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/gmfzbvbgi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.zdbjq.cn/Article/details/gdhjsknsm.sHtML

[I04] 正则替换
来源：http://blog.zdbjq.cn/Article/details/gsqoolyhi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.hesvh.cn/Article/details/ggkqmscuw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/grzqrwamb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/ggzwgkaae.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gpzdckkqh.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gegeadxuz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.hesvh.cn/Article/details/gsttbbdda.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fehbvm.com/Article/details/gwsjqzfct.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/glvhpuyhx.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/gqbbzdyce.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fehbvm.com/Article/details/gnqnacdlf.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gojspmdyd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gqiuriqxu.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gpzthlztp.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.zdbjq.cn/Article/details/gsyzigswe.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.hesvh.cn/Article/details/ghsagyqbm.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gdtwezvzx.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fehbvm.com/Article/details/gnyzktajr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.hesvh.cn/Article/details/grdsbavqk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gqzmftota.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.zdbjq.cn/Article/details/gnccxqiyw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.zdbjq.cn/Article/details/gylsqarkk.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.zdbjq.cn/Article/details/gmhwubdhh.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gociitbgh.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.zdbjq.cn/Article/details/gzsxcrcqr.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/ghhqpaksn.sHtML


<!-- 参考信息 -->