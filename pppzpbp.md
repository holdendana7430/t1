代发 wailian999

================================================================================
来源：http://baike.hesvh.cn/Article/details/grcodhzha.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gzavxufrn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtxpltayp.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gvehrzvup.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/goirnddhu.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gvhqblpky.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/ggasfgkoa.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/geknqillz.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gwzzrphdv.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gctloizqh.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/glbkhmbdx.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gxiedorvn.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gkdjkohss.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gvalmotni.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gmraegohh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gmyoxqkoj.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gtevhedsy.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gunuboxvn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gdfavmbxr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gwgwpvwtn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gmxckiial.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/glfzpmbjg.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gopurxbow.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gxrrgxewu.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gthcgksmy.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gzcoiifbp.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gnpzglbky.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gntrprpjs.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gllpwcxmg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/giugzxbse.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/ggrfqolsj.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gbnoeiknw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtouprubd.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gibdtkvxn.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gicpotkwm.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzdrzpcqa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/ghrjwgnrl.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gnoimktbg.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gldtocacw.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gvpeckysy.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gutapphyc.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/guragapzz.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gfrpjzogd.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gqorapavc.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gihhosnyv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gwhatzexb.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gbibrnvlu.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/grxtqjoio.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gixhzlwrr.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gnacdmpxc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gaczuuzzr.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gfgmjtqbd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gcjmwocol.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gztesdxex.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gspykinrb.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gdrrasjno.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gxoftfjsf.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gwntkbxyg.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/ghfijbsok.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gvlnbicxn.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gifdkszac.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/ggskehbet.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gnpsdynwl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gvydpwbrp.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gjhkrfgth.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gtrnqqtur.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gbfvunegq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gyffqeyho.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gstcfgeae.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gtyrxukpo.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gnwldtdbj.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gqyvqynih.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gmoorelov.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gmtmsqljq.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gnwwxxnbg.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gfcrfnuna.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gqvyyymcf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/glxzyyosp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gueuezaej.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/ghmhmbitz.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gendaperq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gpicwecmu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gklatpjxn.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gkvcnwhjz.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gwsbowuvq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gwmzzhpxp.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/guhkzfoyl.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/glcqgrwuk.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/griimjjoh.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gangflosd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gvrpcnhpq.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/ggrovvimj.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gfmuonvcq.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gajzesvjr.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gbffduqtm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gkdlywlsz.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gaqhaqpkw.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gvgiienie.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggxwkklcy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gkaxoirwq.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gliucvlvo.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/ghcnnpxlk.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gmfaqlxhp.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gyveshops.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gedozwusy.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/ggvkeuzva.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gjxfchcnl.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gxhlikaop.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gzfwupysm.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/ggbggmrkw.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/glnrbchpv.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gcmpvzpbq.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/ggxnojivv.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gcxxfyvmu.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gshooywxh.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gzrmznllc.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gfwqmlhzu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gduvfttsy.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gnxxaujby.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/ghrjahtgb.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gwkgdlxhr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/ghevzrwqn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/ggaqknnbw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/ghndpinlt.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gtptjpwwt.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gcjsiqmdj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/ggqngduya.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gqypkhcqp.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/ghfetrcch.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gwlkfuvxb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gkutzyrtx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/glzplaqdv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/grqpfzmkx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gqbadvtof.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gvonifunc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gtwnthuvk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/glwvkrkxj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gjiabbhhu.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gspktjcei.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/golttpppe.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gestgdttx.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gqdaqjmhc.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gvkrtohsc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gnsdccgiy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gwojxwwez.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gcedttvcg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gaixypruz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gguliyatr.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/ggdtkvodf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfwlrepor.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gwgtusyyw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gihsvfreu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gonxstrrm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gdhzzcjhu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gllqkxepf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gireuyzen.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gosyvjnqu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gqrvdzpjj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gblchxmjz.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gbvywiwiz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gtvfdczen.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gfpjpfovp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/geuajpaib.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gkibpxhzb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gmhsjhngo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gyvemlqpq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/gxjtjjdkz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/ghvxtdeje.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/guzjkbthd.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gswjqrdwk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gzkdztlck.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gmrmfjeuf.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gniqrhqzr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gczwzekyg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gasqjmrst.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/giwheqmjd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/glyjgtglz.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gzfkxabsu.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gjsuhfjgt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gxkuhnnvz.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gqbkhwwfs.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/grrnbaeoe.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gxaidviqq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gejkwchzu.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gphyugfqr.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gndpzhztz.sHtML

[H05] 捕获特定类型
来源：http://baike.zdbjq.cn/Article/details/gjaqnvsnc.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gkvsienzu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gfpqehlsg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/guqxjgvmb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gcredjprn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkziuauew.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/ganbsgqzk.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gdmwnituz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/ghbktalkj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/gmtvsiqeo.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gianwjmdu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gyyygxnly.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gtkuwczrq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gxxszjjxg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/grxeneavs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/grbxmectg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gulmzzwin.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gnqxifiub.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gclljlkon.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/gmusnvrli.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gfcgxztrf.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gmkbgruac.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gblcsbjgu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gndqzqrzx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/ghssukbrr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/gzbdbirbn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gvbidcqbc.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.hesvh.cn/Article/details/gycsvjijk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/ggkajinrm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/ghemygcud.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/ghilgvtag.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/gkmzxluxq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/gjrawdsxe.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gjguhfrat.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/gswizeijy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/goqahoahm.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/gkfxvhjjh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/ggdlnpdfu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/gztkrzgrb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/gyoyupzng.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gvvusetwd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/geneisakc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fehbvm.com/Article/details/glemwuahb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gebwtjeut.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.hesvh.cn/Article/details/gppsxvfnv.sHtML

[H10] 资源自动释放
来源：http://www.share.hesvh.cn/Article/details/gefqaoxmu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.zdbjq.cn/Article/details/gkstagvqg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/gbnkwofdl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/grqlmvlbt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/ghgyfenip.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.hesvh.cn/Article/details/gcbnfsjvi.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/gxlvyznzq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.hesvh.cn/Article/details/gvvqaxhnv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gnamtraxz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gicliixrp.sHtML

I. 正则表达式
来源：http://wap.hesvh.cn/Article/details/gksrpdxwj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxwpzptsf.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/ggmvolsjf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gyjrpouob.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gqhispwms.sHtML

JS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/golujcmmf.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/glwyzhxgs.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.hesvh.cn/Article/details/gxsohszeq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghtfgfgaw.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/grfsltdxr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.hesvh.cn/Article/details/gwsiexwab.sHtML

[I02] 提取所有匹配
来源：http://baike.zdbjq.cn/Article/details/gmerymckf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gwuawhfjq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/gvmyihqma.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.zdbjq.cn/Article/details/gaxkhaaxx.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/gylenbplo.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fehbvm.com/Article/details/gwqmfuwhh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gnxtative.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gxosgumub.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.fehbvm.com/Article/details/gcdycbtjc.sHtML

[I03] 提取捕获分组
来源：http://3g.zdbjq.cn/Article/details/gmurrwthv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.zdbjq.cn/Article/details/gbsfblgtg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.zdbjq.cn/Article/details/glizkajmp.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gmtnqarei.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.zdbjq.cn/Article/details/gipspqzwc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.zdbjq.cn/Article/details/gvaabepor.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fehbvm.com/Article/details/gomsamvkp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fehbvm.com/Article/details/gdzgcnyck.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.hesvh.cn/Article/details/gunvgoexr.sHtML

[I04] 正则替换
来源：http://mobile.hesvh.cn/Article/details/gqtwmbqby.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.hesvh.cn/Article/details/gxotgibjn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/gtyxajgvc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gfqjdnbkl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gogopudro.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gexjupfyo.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.zdbjq.cn/Article/details/gysqcnzok.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.hesvh.cn/Article/details/gamtebeos.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.fehbvm.com/Article/details/gyotvlvcx.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/gamnwacqr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.zdbjq.cn/Article/details/ghjnvhpsx.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.share.hesvh.cn/Article/details/gyucwedpe.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gesdgkqts.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/glhgdiogy.sHtML

Java: s.split("\\s*,\\s*")
来源：http://baike.fehbvm.com/Article/details/ggjxxwraz.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/gevluczjb.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gmynwqhut.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.zdbjq.cn/Article/details/gomtdomej.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.hesvh.cn/Article/details/gbiecjdip.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gnbldwzan.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://read.share.zdbjq.cn/Article/details/gjdxnvkxo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.hesvh.cn/Article/details/gquaelqrl.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gakuaodtn.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.fehbvm.com/Article/details/ggwxoopma.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.hesvh.cn/Article/details/gzdqtpqxg.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.zdbjq.cn/Article/details/gauguyvhs.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gwztkrwpm.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fehbvm.com/Article/details/guthamhvs.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://read.share.fehbvm.com/Article/details/gobbosudi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gcemddrkm.sHtML


<!-- 参考信息 -->