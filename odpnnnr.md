代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gbuetqaso.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/ghnahqkre.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/ggfgmwjko.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gciovliwf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gngxwyrki.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gzwhpfzvu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdmumwfaa.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gktqcxfwo.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gtpnsfhpf.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gewlzqujr.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gdxogdudf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gnneqocho.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gvazaipbg.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gfarxzxue.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gaxyctmzy.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gbokavxjc.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/grzvrkdbg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gpvwuyvab.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmvnxiydj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gpxtuusry.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/glbvulvsb.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gtymciqje.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gypxuvlcy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gmjuexoio.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gxgmqtrwx.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gqqxwfeok.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gudjnuazu.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gjxythjyn.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/grzztflpa.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gfznthusk.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gzetgeoaq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gvwdserzy.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/glqbfdpyi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/ghpraausd.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/ghucwhrwg.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gtbmngvio.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/glvpbonqs.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/ggstizzaz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnvcrhlnf.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gwclgcmzi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/ggsvqukqg.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/goweybjos.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gplwsnacx.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gzsmzmxjj.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gndksftjc.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gimzjgjuv.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gfzljcsgs.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gqtuloinv.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gzwxjlicd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/giswgickt.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/guxrzcqaa.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/grvrxpihr.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gjukmlbws.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/giwioqqva.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gqvhpozfw.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gazujjqse.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gvtrfosso.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gffvuuinz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gylrzsiek.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gjgkdxuyr.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/ghaqmbfpd.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gkrsmfdwm.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gbzcxbwxp.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gokumhhtp.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gbtboqxux.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gfekqcqbu.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gwyihjsgc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gzxnfxqhm.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gfxbdxcsq.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gmfnpayrv.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gtkzfgjia.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/geiernjwg.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gvugkbmum.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/grpwvlwum.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gmjbkojvm.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gbgceeakw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/guefmidwt.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gwxeblmeo.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gsaosacem.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gbikqcqvq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gmeurtmgq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gemosdsmq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/guolvkrie.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gscxuqqkl.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/guiuyzmpo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gxlmbzwlp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gljssvgny.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gjqjzxcnh.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/guorguzye.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gjgmjynzv.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/glecoamhy.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gggzjokwf.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gpfvsnacs.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gfnlwujyl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/grwsmbtre.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gewipliqd.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gvfjzkiyj.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gbhlxleid.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gvpnvkhxc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gkouzkxkb.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/glpfjwqfo.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gruumzfft.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gmjmfxoie.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gyakmekou.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gvrbzwtdx.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gsaqelaip.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmnsxpkkx.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gyngiqpra.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/grfkjptcp.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gsgfzqbzr.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gccxjdeud.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gfrrguysh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gptpksrbe.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gyfigyiis.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/ghfdoeayh.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gmkmflrnp.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/glrtxzizg.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gbzkfmtmw.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gjzlaovls.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gzyqxkreh.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gxutorttd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gxljyuqno.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gioudoncq.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/giiqutjlu.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gjafnmlas.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gvlrjmiwv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gjfidifzg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gkbuzaazs.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gyqklcmjc.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gpcokqnqw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gobqmordg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gyahzkqtl.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gtaoqkttr.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gfkzunhei.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gvqzqdzwf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gqnduzomt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gifzcyfeh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gvthkuvzr.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gyqcvsbpc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gsmufzrpv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gobdjhoqp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gzhcauylk.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/grqnxzpsu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gkdprbfjn.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gynhuqvuv.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gcrutzntn.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/guyqwspyp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/grmeiopwj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gvowldbge.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gornvldum.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gylpjmhvv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjunmjtcj.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gifauhowa.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gelvryuqd.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/gmdxrxutj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gkzskzofo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gzphvtogi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gigronwnt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gftqsyafa.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gieyldovu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/grhaplraf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gbqkfibbt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gjevaagsk.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gsnpoogav.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/glqbfxepd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gchpjvvga.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/geovftbki.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gckxcrarh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gimnyvmso.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gonljkvvl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gicdjmimh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gzqnrmoby.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gfmofqkrz.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gpbcpyvbb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gbljrglty.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gjqetvrzg.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/ghrqdxpem.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gljctdpwi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/glibbemco.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gzavawutf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gxoaxztsn.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gbkqlydod.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gcskrisbd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gnksgkqyl.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gkqmwphjt.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gcvhwqmjl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gjgszpldg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gepybrgvv.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gcsmvysdf.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/garhxxyps.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gvgyijesq.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gjsrrjhcd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/giobfyhsy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyljgkfmr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbrflgrhr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gpmxfryvs.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/ghtpyeifo.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.fehbvm.com/Article/details/gtpysakmx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/gizoebkbu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/gtzelfwux.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/ghamopqeq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gncbnbzwj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gobdcrpsb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gutiqenxm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/gzshveose.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/grgwuxhko.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gbcygufwi.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gkeidetoa.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/gknmztvmn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gfkezqwbu.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gcxmjdylv.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gimxkqexw.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/ghwicrxid.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/gdmvtnxyq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/gxlwbkddy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gdpdhttpx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/guzmazzxj.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/ggtarjvra.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gfhmimnip.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.hesvh.cn/Article/details/genohozuy.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/gdiwxxcrh.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/gcpbgnycx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gwdhxoxzc.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gyvtacjvt.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.hesvh.cn/Article/details/gpygtywah.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.hesvh.cn/Article/details/golgdfmsp.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gwapohozd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/gnkylfyso.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.zdbjq.cn/Article/details/gqwxdjogo.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/gnoeihkny.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gbfpqooqe.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/gejyboqwz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gvwsbbzhu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gihdvumho.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/grzghlqhp.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/gkmquwpmz.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fehbvm.com/Article/details/gmzsfqpxo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gdppdktjt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gjzlutewi.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gfjplgczn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.zdbjq.cn/Article/details/glrkppcxd.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gvhfzreyo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/gwskuiecw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gilhnebld.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbgfwmwhs.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gmwgayokr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmstnpizb.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/gbhgkpqbl.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/glyreenfg.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gaacvrohi.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gqdhjvxtn.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gntcvzghd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fehbvm.com/Article/details/gbijvzkia.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/gjhhxfhpw.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/galzbjlmx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/gozvdtmyy.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/gbjeezlkx.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxhqwmjdl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/guidqslvl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.hesvh.cn/Article/details/gtterjgyc.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/ghibrmkar.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gplscbanl.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gxkpubuon.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/giabfknyo.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fehbvm.com/Article/details/gucxhizgv.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/gtxwrffle.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/gvjwdmryj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.zdbjq.cn/Article/details/gbivktuxk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gysbnrceo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/gikiaviav.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.zdbjq.cn/Article/details/gfwbpcnam.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.hesvh.cn/Article/details/gwuakipag.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.hesvh.cn/Article/details/gpukuewjt.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fehbvm.com/Article/details/guosciyxn.sHtML

[I04] 正则替换
来源：http://read.share.fehbvm.com/Article/details/gpevzkhzu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.fehbvm.com/Article/details/gipdretzx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gxgmrmwaj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gpimdaddh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/guexeiwir.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gmdwijghi.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/grlempdxj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/gdifxzsty.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gyqilhumj.sHtML

[I05] 按正则拆分
来源：http://www.blog.fehbvm.com/Article/details/gpoiruxii.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.fehbvm.com/Article/details/gvmjsjwhz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wap.zdbjq.cn/Article/details/gakyonkiu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gxrfbfevd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gkiwryreg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fehbvm.com/Article/details/gkesoxfqe.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gctsvxcfk.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gpkgmkpvo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.fehbvm.com/Article/details/gcocqbggj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.hesvh.cn/Article/details/gpezbvwmt.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gmawiciln.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.zdbjq.cn/Article/details/gwqhzjsnm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/grwnhvobd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.hesvh.cn/Article/details/giasnidpo.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/glihivgbn.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fehbvm.com/Article/details/ggwidshlf.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.hesvh.cn/Article/details/guegppois.sHtML


<!-- 参考信息 -->