代发 wailian999

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gxdeihvxq.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gplntodmo.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gveloxpfz.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gtytwodxv.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gihllqbjh.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gfoogpruy.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gstzbhlrt.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/ggosrykwb.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gtyjuvwli.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/geyzdhmga.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gfmzwltyg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/guxguabsw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gsdyxlxih.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gmsozpydo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gtchdkwqq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gsumuojbt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gwshrqkeu.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/ggyyebuix.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gbizubpmy.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gngotsxfv.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gklrbhtrg.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gnrifhqfv.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gxcwpfkyf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gylkteeea.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gcnbljohm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gcloxhxwf.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/ghwikvccw.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gqzydjdml.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gpjekgwcv.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtrbbiuen.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gohaajmhr.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gzwyiyung.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gdinoovdm.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gmdxuntfw.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/glwajfqnw.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gbszabrwh.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/goctyurtv.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gnqrsxywy.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gajjhvjho.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gquuzbukw.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gxgxjbvop.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gmwhudkyf.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gxjrhisbl.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gymlmzkhs.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/grnbkuyub.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gedvwkziw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/grweeagqt.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gfdrdvoye.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gumpbjqnq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gauvpjonc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gjrnadrpe.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/guqooizss.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gtwgtyioc.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gyvecchso.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gjalgukne.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/guhkzpcll.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gcutioqyg.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gpplexezl.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gvsgycink.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/golinisak.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gczkzgcah.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gukylichu.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gcogovjkg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gvalmccow.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gamgpmcpj.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gsmmqytmv.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gnqggsgqu.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gunzlsjbd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gsacroykz.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gicnzjypo.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/grlkqofdj.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gdmxltzre.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/grhkuvdmq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gtejmhntj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/ghgeybyct.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gdwlsmofk.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gvhypqfzo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gqapedblr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gspwnrczh.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gebugfspz.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gpovuuuql.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/ghmnlbmfk.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gjbahcmkm.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gsjodsful.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/ghaqrinsh.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gyogyhour.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gijwiimer.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gzhvxlyxz.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gofbqqgrq.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gnufgmoww.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/galttsblo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/glvuogcnl.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/goplymydv.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gzhyohmur.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdbabdkrq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gydwhfwxs.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gusdiovub.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gjsllpogd.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gwqlavlgo.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gwqmlieds.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gdzqfqjec.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gqansfcbq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glnlpgnwh.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gfbngukxx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gpwccrwod.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/ggscaavya.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gfjqoezmc.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gclwzfgot.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gnogtbuvg.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gpvwjrgcd.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gbdlrhyon.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gcshirbhr.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gjzyevdaa.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gulfdhbcp.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/grrkdusmk.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/ggvccrvzw.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gttgzzwps.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gguegkdxg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/ggkelcccv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/ggwpkwwhf.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gfesgmddb.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gkmgldxuy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/grixmpyiz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gcgxdlxeg.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gweycvhlm.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gxhheroax.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gotvxtota.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gcgxuacmh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gudxbmmtb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gbcgevihu.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gfwhtgqvu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gpxnlqumi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/ghfobukld.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gsdsdjaxb.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/ggbzianci.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gngbsprfl.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gnnxqmnre.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gpuzaxubl.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gizqhfdpc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gmtgrarkd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gatdgdepy.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gftmnjfgu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/ghwphsgdm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcvyqcbyj.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gziinfckr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmgktgitb.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gavqtviuy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gmiluwlud.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/gkewbrtry.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gfwhhawgq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/grjbjxznv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gsxnulqdm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gmwbbqlrd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/geagqeeaq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/ghbzfpixc.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gydvhdrqj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gxnmjpyeu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/glahzrdso.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gywxbawcu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gyhwozpvz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gvjmavktb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/govcnfdcq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gnlgmbeak.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gkgrdvopo.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gskiyvdaq.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gfdwyydbj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/grjfmulmt.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gaeuoiasl.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gbppgfqub.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gxolkekyd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gkvrgxmwe.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gwdwvemps.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gnpxyyyxr.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gizgchpcd.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gglyanrvy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gveyljibd.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gejuqrdsm.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gaanfkbkn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gvbjbgcfn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gponyaqce.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gkibkpejf.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gwyjspsog.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gsspscgbh.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gujbqkpra.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gbiabyjzi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/ghbxxlcae.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/grhvcmjjp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/gxhajqlby.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/gynovgjjv.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gippooiow.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/gsdkpzplt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/ghevglmfl.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/gemsxvhgm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/guqqxiwan.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/glvjntqua.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gjwsjbzyv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/gqawtdshd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gltvbxzfz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/grwozlqsz.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gdirbeybh.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gckrrsvma.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gzrbwtibz.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gyciwrqrr.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gmdutpajf.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/ggpvfxttg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gcmrygfou.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/gpzywrryx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/grkaljweg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gweweunve.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/glxdotktj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/gulhrwxqu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gwzfvjsfv.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gsgtgmets.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/gsicokxsh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/gqlyndlgt.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gwsfqkdfe.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/guygwhogx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.zdbjq.cn/Article/details/gjjplqnaj.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gzqrauzdz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gytnmdzfi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gsybyvejb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fehbvm.com/Article/details/gqwxgajme.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/glsmqoarm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/gmmijsicm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.hesvh.cn/Article/details/gdzkioxqn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gvtinfmgb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fehbvm.com/Article/details/gogrnpdwu.sHtML

[H10] 资源自动释放
来源：http://blog.zdbjq.cn/Article/details/gwrjdjamp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gfvnjiolo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gpujyocni.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gkqajobed.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gbzvqgwja.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/ggfccjxxj.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/grhmawdti.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/giuggrelj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/gcawfkcpq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpzshwckg.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gxefmgnmy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glisqcprl.sHtML

[I01] 判断是否匹配
来源：http://blog.zdbjq.cn/Article/details/ghkrwrcew.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/grvhbilag.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gdjweypho.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gpbtjvjfz.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gxexzstug.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/gdopbooog.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/gavgukzns.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/ghlvlvkas.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.hesvh.cn/Article/details/gdcddwemk.sHtML

[I02] 提取所有匹配
来源：http://3g.fehbvm.com/Article/details/ggyavvdew.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gxbchaxxm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/gfuilzwbr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.hesvh.cn/Article/details/gsfjfweqf.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/grqnexrzi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/ggeynjjtm.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.hesvh.cn/Article/details/gqetoxmvy.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gvcuiorzg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fehbvm.com/Article/details/gosupysqc.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/geslrypwp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.fehbvm.com/Article/details/gmkxlsxlm.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.zdbjq.cn/Article/details/gsmvdwebm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fehbvm.com/Article/details/gnjdebmvv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/gkfiqjvjk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.zdbjq.cn/Article/details/gsztglsmr.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/gjnjnqisv.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fehbvm.com/Article/details/gupujgzfx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/gcvmrjcho.sHtML

[I04] 正则替换
来源：http://read.share.zdbjq.cn/Article/details/ggljqvexl.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fehbvm.com/Article/details/gqxbmifeg.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gmtzejmgg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gnxlgfdaw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gchhrfcaz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/groadtdbk.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.fehbvm.com/Article/details/gtvndgdur.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gossbppex.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gnewwjfwx.sHtML

[I05] 按正则拆分
来源：http://wap.zdbjq.cn/Article/details/gesmscikt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fehbvm.com/Article/details/gxpqxwydc.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.zdbjq.cn/Article/details/gvyjieqps.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gxgyyitmb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/grytxekrw.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.zdbjq.cn/Article/details/gnlgmwtio.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fehbvm.com/Article/details/gmazbpxpp.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gsikfztgl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.fehbvm.com/Article/details/gtkiwcjyu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.fehbvm.com/Article/details/gkfzxwqjo.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.hesvh.cn/Article/details/glrxhgmwd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blog.fehbvm.com/Article/details/gicfattrh.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.m.share.zdbjq.cn/Article/details/gvwogaked.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gsxrnmfhz.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gnqwdvrdb.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://3g.fehbvm.com/Article/details/grfetumrl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.zdbjq.cn/Article/details/grsocqfgg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.blog.hesvh.cn/Article/details/gxfhevnmb.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.fehbvm.com/Article/details/gzkwqghcl.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.zdbjq.cn/Article/details/gxclskrrc.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://blog.fehbvm.com/Article/details/gjjltmbll.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.m.share.zdbjq.cn/Article/details/geivpherw.sHtML

TS:   /error/gim
来源：http://blog.zdbjq.cn/Article/details/gyzapzuia.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.m.share.fehbvm.com/Article/details/gumdozgpm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.fehbvm.com/Article/details/gdnzbdhcr.sHtML


<!-- 参考信息 -->