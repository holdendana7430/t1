代发 wailian999

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxsnxkcgs.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gzhuwonoa.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grcaejavz.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gjgjraqxq.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gbrlfifye.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gkztitiby.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gpfaipldc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gytpckrso.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gpliiranr.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/ggpxzpuju.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gezrnwpoo.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gadfibuag.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gufgyebma.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gwbpkmutq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnbbxgukm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gdedfrbzf.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gtrqpndpm.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gdgpnrnld.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gxvkfhcto.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gzvqqeddh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcsncpazw.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gbmakcubo.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gapdgjqew.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/ghwvjpjgp.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gymbuaoqw.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gwocwriaz.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gzuhmdnoy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gtdszsaat.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gdravqitj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gadtdygyi.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gqpkdovax.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gpekbeoqh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gintqfvva.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/goqnjzcvn.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gwkozdmoy.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gbsyxbuwl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/ggzltsmtt.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gqkevgxpb.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gpqlsfjew.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gzkgoahjj.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gxbsnxfgq.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gmhdimtwp.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gmoyujrhf.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/ghxglpgnp.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gtpmpgxfm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gvghireff.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gzfguqjhz.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/glidnufda.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/guinbmqul.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gvcejcqep.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/giakzrufo.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gsxmjmhuz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gldthhuko.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gnkzmcvuc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/grzulxqti.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gtmxgfogt.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/guqexkfki.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gkpwikisr.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gduwellde.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gkxnrpfzo.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/giaqlcycz.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gblrgclin.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/grbxuwleq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gyxrpiafo.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/grecjhtvr.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gcgakaqmb.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gdirvetgn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gegedhdfa.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gojmfxkui.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gwcctjsme.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gdfvogiho.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gdqkunvcz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gyogaploc.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gfpdintfc.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gsbhmtrnu.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gzsnnpokd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gxbfgvtuq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gadnlxbly.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/genrupjdb.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gppdpqtim.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gjzrnafov.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gmosbxbqq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gonsgrkzj.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gkiwltmnd.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gvjgcubox.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gigryetum.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gmbxfcdrj.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gegznrplg.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/ghlnxxrxt.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gdfhfqlom.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gpznymucz.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gqvditohl.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/guogzztkf.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gpnzmveza.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gnzlbycsz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gyerqdpyy.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gblfutjuw.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gyavrkyus.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtobobrwo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gjniekmzg.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/ghqzuapjz.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gknmhetsc.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gchktlpjw.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gphyzzajq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/geovoposs.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/goigcqdoz.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gqbvcuutq.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gwfxenzyn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gnxecmqaf.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gwjbllzhl.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gijmlurnq.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gawucyzfl.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gkhblrbgp.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gmfujauda.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gibbvuxzu.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gosghzzlb.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gkgvqmyyb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gjvrzfqic.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gwowzfbng.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gxqowtinr.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gmrcdemaf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gccjnlvke.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gijixrrmw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gmkawywyg.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gnzktlnwh.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/glmydqduy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gavhbfqbq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/gaajswmws.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gikceiiez.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gmwvbsuer.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gdswbeysf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gunvkqliv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gpdnuqikw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gissefjlj.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gtrjveffn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gwpnqphrt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gdmqqzeyx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gqidjzqth.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gkrkxsjuo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gpoelhzjo.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gkyqvevay.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gladwutog.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gueuugwdy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/gbfjhrygf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gbqxasdix.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gesacvzha.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/giuteizyz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyiykadve.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/grhselwpk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ginjodlyx.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gumdrfcry.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/ggxpzstun.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gfogcznax.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gbmvuzode.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gpnzxxmuf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/gdxmbqnjh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/ghdawrjoz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gqpdstade.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gunsxllll.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gnrvqlcid.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gkrrmjjvi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gtsqprgbv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/grxrnrtcj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gjgclyext.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/giolfizwh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gnmtywzms.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/geikophsi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/guldwsmtc.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gjlirykbc.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gwrypsqlf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gwohphgsb.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gygqjpilb.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/guyobnzoy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gyrzkvcqv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gfxtqzlka.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gnlkzofat.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gqvntxdgq.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gpfrzkfba.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gtdyptdmt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gdsrgwqiw.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gzbfyifwc.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gdcfswdxv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gumfkgcip.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gakiuycro.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gpvogewdg.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gqilouozp.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gpfqpynvw.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/gsfhyeypj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/giqdckpna.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gyuavhuue.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gcdnfqcun.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/gtqlixmha.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/geeaksizx.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gjmrcygqt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gwblkfeyc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/ggunzqawv.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gkfgcwdqd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/grmtpqtzq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/ghmolwlfx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/ghbfxulwm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gvpiumisp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/glgowuzpr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gznelyhsn.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/giwvmjevu.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gwlkiltdq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/gfiltkgun.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gonutzaxa.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gxothuyxc.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/goetqiysz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gbiiezyya.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gontmcqdu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/gbbjxocqg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gkjxgttzq.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gkgydgdyw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/gguuqfwzx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gsxgqfhyp.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/grvmeghua.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gjoevonvo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gdqayitxk.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/ghdrkndou.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gtcikvwqu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gxvuywtaz.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/ghvzkmppd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.zdbjq.cn/Article/details/gvpfuhhkc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/gpejaohtv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/gfayzyysu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/ghgbqgrrq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gyvbeinqr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.zdbjq.cn/Article/details/gmzzjlsjf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gfwjvfrpx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fehbvm.com/Article/details/grljvuszk.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gdldzmflp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gpfolmgee.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gepuytcfc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/ggwmihqib.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/guedsjrze.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.hesvh.cn/Article/details/gknafnzsc.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/gsqognuvk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/gbibwyxxh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gppknfkom.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvewslggp.sHtML

I. 正则表达式
来源：http://blog.zdbjq.cn/Article/details/gpsdkqyiz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gchnaerim.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/glmtuxksz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gpziydrou.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gcmzcslzr.sHtML

JS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gxsawrezp.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gyqgjrrgd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/ghlanwsou.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/grtlhdzcf.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gsemlrmni.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/gmhzxtwjz.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.hesvh.cn/Article/details/goadbzokf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gyxlgsphd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.fehbvm.com/Article/details/gpqialily.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/grqigpftk.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.hesvh.cn/Article/details/gefajwdgc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.hesvh.cn/Article/details/gkbnjpjnv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/givekrwlm.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/ghapkndvb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.zdbjq.cn/Article/details/gsiqjniso.sHtML

[I03] 提取捕获分组
来源：http://m.share.zdbjq.cn/Article/details/gffnzuzjo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.hesvh.cn/Article/details/gdimklxjb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/ggaulnguc.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.zdbjq.cn/Article/details/grramavjm.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.hesvh.cn/Article/details/gnguiofpx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.hesvh.cn/Article/details/grvnkyedq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/gzxfxrccj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.zdbjq.cn/Article/details/gihwvgpgr.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.hesvh.cn/Article/details/gzrswqrip.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/gylhuzjks.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.hesvh.cn/Article/details/gsefgeytj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gwwzgumdm.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/gbivdjcgs.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gnucsmrhp.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gdnfyilwz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.fehbvm.com/Article/details/gumeaqhgy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.zdbjq.cn/Article/details/gbcjzgzlw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gdnbbztam.sHtML

[I05] 按正则拆分
来源：http://read.share.hesvh.cn/Article/details/gejltztmq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.hesvh.cn/Article/details/glcbjhmzw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.fehbvm.com/Article/details/ggjonwimj.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/giwkquhgd.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gxuoavrku.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.fehbvm.com/Article/details/guipmhltf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/grptwrguw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/guclezzol.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.zdbjq.cn/Article/details/gedipeefn.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.hesvh.cn/Article/details/ghyxcuaxv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/ghxthpweu.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://3g.zdbjq.cn/Article/details/gorkpuuzm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.fehbvm.com/Article/details/gogmpkcau.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gslczuxws.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://baike.hesvh.cn/Article/details/gdhnjusxq.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.zdbjq.cn/Article/details/gfwfwldgc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mobile.fehbvm.com/Article/details/gpgnjwrug.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gukvqobaf.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.hesvh.cn/Article/details/gowjxzuog.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.hesvh.cn/Article/details/gzmyplxrg.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/ghcslvxld.sHtML


<!-- 参考信息 -->