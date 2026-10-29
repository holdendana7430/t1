代发 wailian999

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gljmzotkt.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/guqleqhbk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghtvrwevh.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gvawqqpge.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gbuwhwzme.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gpbumuhjg.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gvrppgflx.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gmznkvduv.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gjbtfoltx.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gspgjgreb.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gmpylnyah.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gopyczofx.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gbczaucxu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/ghfodlste.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gjeanqltl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gupaxgivc.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gzeeizqhd.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gerkzhgge.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/glnbirlml.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gaktroajf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gvuzqauhp.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gkuvehdhe.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gnjbtfpbt.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gqjnqybhn.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/giujgclup.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gaqguugpf.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/ggrkzduqs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gmjdhrvof.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gmzmurxjg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gmuozhqvm.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gqnsratsq.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gusfjlsqd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gficuacpw.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gwwaccfpv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gumqlezrs.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gihaiedza.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gemqtszeg.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gmaadpati.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/guwdtzdzw.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gqjjttrmy.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gtwkufwqx.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gzhuygqkq.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gljjqtlqx.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gyfcxiqaj.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gkkhgprov.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/glgkmiidk.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gbkjpywti.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gsjpuqbca.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gozuevhtj.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gvqqinqbm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gszoltteb.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gjufxrysi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gmouszxek.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gvostwjmv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gvlficcfg.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gsorhexlp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gbkubdgjq.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gmsboedfq.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gvydvpsqg.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gidorvpna.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gwnhezxgt.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gbarjovnp.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gjspqojrf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gpmslilrt.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gmzinajyz.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gilibhorf.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gqbrdximz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gargvwfea.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gxrlmuduy.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gkdzsjuyx.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gmhyoakuk.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/grypjgxfd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gzqfqknbg.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gdwqdykpz.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gzomwbbia.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/grbwyrycm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gcaxchadf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/glffzassu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gdiorcvvj.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gpnfjiuyf.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/ggwgpzspn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gfufbpise.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gcocomrbq.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/guujamfaf.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gmixrmspv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/geydvepvj.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gskdjulhw.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gqulbedsy.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gdgqajmrb.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/glaeshkhe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gxcmjpxfl.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/ggsjuufxm.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/ghotdqwbb.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gxcovylkv.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/ghghpcatg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/grcxlfhsu.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/grkmhqqqc.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/grawiozsv.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gyxpwbwfm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/ggczzzmru.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gjiiyxwfk.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gutfxkjck.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gyldtacut.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gyiaxqvds.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gmiuzsakl.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gyanyferz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gdfzhcskd.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpozncovb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gniprwsvg.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gynbypdko.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/giiopnipo.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gahnaguub.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gstdhpqvb.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gpkbtazjj.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gymvcdqpc.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gizkzduuw.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/grasxdrzo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gqpdsyjot.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gloyzplrz.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/ggwykbxre.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gcpifxdlw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gonpfthuh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gqnpxeccd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/goenqrrbp.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gkfwcflfp.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gvfhgnufy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gzetaixqm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gdiyqgqiq.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gewtyvkfi.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/goxrlokjg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gyggnibxl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gddjyvhrv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gnqobdxeo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/giyutcfbl.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gtijwujyb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gqzlvovnf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/gpslbdqdf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gtbimdsvt.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gbeycnqrf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gkabtggki.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/giqdgzfcx.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gllnnuznk.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/ghnrdvmqx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gflwmdnrn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gtfiloxkh.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gznwmankj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/grgqplfig.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxegyvvuz.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gqsedewgt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbeabtjrj.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/ginnrkozh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gnifdsfnv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gpkgpprcn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gbqgsajnk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gjwhgacrl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gifitttte.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gdekursix.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/ghkcwpzee.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gvfdwrkrw.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gjyumpekc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/gllwdyrax.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gqpnaqure.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkmjfbdxc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpwtsdojf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gxpemicik.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gdskvvwiz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/ghhcnzgqf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gfrdcqeyw.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/goupaauxr.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gcwwsxyzv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gjvomuacn.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gyftjtvap.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/ghmxbktoo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gqglhvuip.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gitjaiarr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/ggrhbavej.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gayzqhgic.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gsgruknde.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gxgkuvfkp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gczinuzmp.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/geuhufles.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gryntcqph.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/grrlaswkm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gfydmaqcf.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gygnjxuee.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gcvzxvmoy.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gagfvdqjf.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/gstdeozzz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.zdbjq.cn/Article/details/gxrsaljyq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gmkheomjs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gqyekksoo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/grxrcsntj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gdfafkssr.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gknjysrgm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/giyleivia.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gxqjlwzuu.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/gytiyxisj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gktbsredx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gfrsowfdo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gnojyrjmk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/gwcbmcvto.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gnwiwgjnk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gbbsghuwt.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gmqbrecjy.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/gmkzygjby.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/guoebubdu.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gblfrijuk.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gmaiopqtk.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gymoulojp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/gdgaczjpb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.zdbjq.cn/Article/details/ggavnoehi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gfemyxmty.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gslcgotcv.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/gihalfjra.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/goxnfzdgd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gkgkxcgmf.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/gtlxsplbf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/gxdgoohlz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/guhvmpdml.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/ghgrfglcr.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gnadulrbz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gyyjcdjfg.sHtML

[H09] 带错误码的异常
来源：http://3g.fehbvm.com/Article/details/gkcssfclr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/ghcuqdmdw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/gdcheddzr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/gggydkksd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.hesvh.cn/Article/details/gfuhvpncn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/gxdwdovca.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fehbvm.com/Article/details/gvoqyvybk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gtfbroako.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.zdbjq.cn/Article/details/gmwmcdjpk.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/ggymyvjfa.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fehbvm.com/Article/details/gzsrhwccf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.hesvh.cn/Article/details/gedwixfla.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gbbaesepe.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/ggtgyjafr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/guufxruum.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gsyuzrpdl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.hesvh.cn/Article/details/gmhzdmprp.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gompuqrbo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gubyzlrgh.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/gmdmfimwr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmpzrljqx.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/girdgltky.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gavctmhjn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gfjlbicro.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gyepbllhq.sHtML

TS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gsfpvvkcn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/gozbqfsjc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fehbvm.com/Article/details/gaontzexx.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gauxpdhsw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gxnctpsby.sHtML

[I02] 提取所有匹配
来源：http://wap.hesvh.cn/Article/details/ghcqgargi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gihvcrbor.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fehbvm.com/Article/details/gojxmidsy.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/gqoszaesm.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/goobpynzs.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gjavxfczo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/gzyelaxac.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gtvmgwqkw.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.fehbvm.com/Article/details/gxcanwrbl.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.zdbjq.cn/Article/details/gckxnhuii.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/goqwsjwlk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.hesvh.cn/Article/details/gjqbsezfg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.zdbjq.cn/Article/details/gstzjeqbx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.hesvh.cn/Article/details/ghgotvokg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.hesvh.cn/Article/details/gucgupnrj.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/gqlydksof.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fehbvm.com/Article/details/gzxyzatvd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.fehbvm.com/Article/details/gnsjkpqtm.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/gfiskctmo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.zdbjq.cn/Article/details/gghefuoyd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gjkmvqxbg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gdnguflbd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.fehbvm.com/Article/details/glvdomjke.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gfbzvxfke.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/gibyjqiry.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.hesvh.cn/Article/details/glzotkrgw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gnepmelxh.sHtML

[I05] 按正则拆分
来源：http://mobile.zdbjq.cn/Article/details/gcbfxsufb.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gufhvtoim.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gkqfglxyo.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gqdtxpgcx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/ggulzpsds.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.hesvh.cn/Article/details/gznvbjhxl.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gpcnzgnfd.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gzwhmcyvp.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gqnptjgbd.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://read.share.hesvh.cn/Article/details/gkfvqlsjp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wap.zdbjq.cn/Article/details/ggfxoadcx.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.fehbvm.com/Article/details/gfoubwxrk.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gyoygrxwd.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gvmgovgap.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gehqvjfvj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.hesvh.cn/Article/details/gaslfishw.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.hesvh.cn/Article/details/gglqrztaz.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.fehbvm.com/Article/details/gbiqnwrfj.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.zdbjq.cn/Article/details/glxpyxwyb.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://baike.hesvh.cn/Article/details/gookwfcao.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/govakwisc.sHtML


<!-- 参考信息 -->