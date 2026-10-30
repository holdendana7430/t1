代发 wailian999

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gfceiehfg.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gaxqripul.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gxbwmwjqe.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gvnhrawvl.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gqeuilazb.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/geksgrxle.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gcoapvdxx.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gttchdgnn.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gkhhwpgud.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/ghodpkrim.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gzckwcylf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gouhaspcp.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gqmzqxagc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gxnshtldx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/ginyhktkk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gytzgarqv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gbofgiveq.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gdxspxjns.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/ghofwyjid.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gxvedblyw.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gqzsztefw.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gypiagjll.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/glaicevtx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/goucjpmjm.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gjlioipjp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/guksaesgz.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gvazcpplo.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gawsjbhvv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gfbqjjhsf.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gbcayvgie.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gwkyolops.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghfjojiqa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/geppescje.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/ghmxlkyhj.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/groymuerl.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/goclruudw.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gaksfzkcb.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gmubvrbcc.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gqnqbpklo.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gcdruuakd.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/guqamhxzo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gcouzjmun.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gayfpjuqz.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gifdgopjn.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gawnvagwi.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gbdatxkvt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gzvpczvav.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gpywwwikc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gdewcbrwo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gcegehota.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/glwvtofkf.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gppuyfbhi.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gdlxkrtxb.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gvrhjiykq.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/ggsnahxhk.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gyyelkfpm.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/glwyyomlr.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gjhpxxmvm.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gvivllhoc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gdftdmosk.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gzroofuvz.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gijkazqqe.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/getwogjip.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gxtcnbnhw.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gflwbwwvl.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/ghpvdwihx.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/giidnhicw.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gqmzxfdnp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gtcgwjwuf.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gmgdhqxeh.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gsiokcuvd.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gnfaaiywl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gatjlqgdp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gpvnzraya.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gtsibetui.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gnoedgadb.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gktstuygz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gqhbfvjke.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gguebbrbx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gvcnsamgv.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gmbntysyw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gxhcsckcr.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gstwsvoxg.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/ghzjghkok.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/garewajeo.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gbxwidxfa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gcvnpszgn.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gxahrbinj.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gkijedxoy.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gxoanuxfk.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gazmwspnk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gtzuygftz.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwdmppfmi.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/goduuhsru.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghhwgqfgu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/giofkrdlm.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/ggsodbbmg.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/ggrzruere.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gwifvexza.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gypmhqcyz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gmgmbchso.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggbxlwzuh.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gtoztislv.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/grtoqmouk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/ghemtmopm.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gljszcsvv.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gjmvjxgxn.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gfbuptavb.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gznblaqsd.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gakddywln.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gtmhdtfhv.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gxnvaltut.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gheceakhq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gggxnnsuf.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/goqadlvcf.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gijrcbqjx.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gxyfwjdyo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gfvikxyvh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gpvjoryza.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gbjupgwyl.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gwpfbvuyx.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfbdfjbns.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gizdzpvvc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gzciapmut.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gufybjqcl.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gmlmhfmjd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gfmnukfsx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/gukmgiqus.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/grtonnlzu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gxionezah.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gtddgdcmk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/glzhhibhw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gdqhydzaq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gkkbdrmfv.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gjxxarbwf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/guxrsmmaz.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/ghnsddxvr.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gzywqyxdk.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gcdropxkz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gejatrhjv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gylewlloo.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gdugunxqy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gftrabtfj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnsbebofv.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gmxboklaz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdtokrlbs.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gftmtchda.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/ggyododpb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gqwdxsppx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gioflelhh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gobzhiqdc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gpjheavlu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gfomyktfu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/ghxmajzfb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gganihrgu.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gdknmocca.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/gbygliykk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/giamgkoga.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gcsqzevnb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gtudiwpfh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/geyrvzvwl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gbsrgmpjt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gtihhckhg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/ghqtvzkfl.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/ggampydsy.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/garqjnvht.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gbfzcgrvx.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gypwoqxbw.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gnpmrnlrv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gsvtbfzzj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gejbsinar.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gkvlhoepx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gocazxukz.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/gzguqpjaz.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gftrnzwre.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gspthbrod.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gladyjhzw.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/grmwrlede.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gdiwujgcv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gzzwoggdi.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gdlvidmrg.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/gnewjhqlm.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gufmjxyys.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gubjcomzg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/ghevznilo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gprqeatnf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gnkkzczfj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gllnjkgab.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/glyudlynf.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gwpwrjxqg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/gqfxboxwr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gkhrwajfm.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gozmmgbry.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/glqtcmicd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gihfovgel.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gmjwvdwrn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gwdukscwk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/ghkseoemk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gjwolpbpi.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gvuojtltn.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/grvhiivhy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gtbsijinn.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gsapukrxx.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gmqppkkqi.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/grmyhnrko.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gumujnvva.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/gjjxjixjf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gsyaevwnq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gbsucvxfz.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/geyhlochp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/gimpdgfxy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gwbqqawzd.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gvinxbwds.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gmmglsdet.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/gsrgzwosf.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/gidxukbms.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gklhynvnc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.hesvh.cn/Article/details/gkxzglaju.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/grjwghhgn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gmgqmenrq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gccnvszoi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gsvmtqsri.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gevoqppas.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/ggsyxqdnu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/glcvfeepb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/gjdefcrne.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.hesvh.cn/Article/details/gmdydzwbu.sHtML

[H10] 资源自动释放
来源：http://blog.zdbjq.cn/Article/details/gzskawdnt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.fehbvm.com/Article/details/gbzoyhhyt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/gyozdqnqy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/ggdqgoflo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gmnknlynr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fehbvm.com/Article/details/gzmuoldsf.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gedqheuoq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/gfzppywby.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gmozlrcky.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gacmoqxqe.sHtML

I. 正则表达式
来源：http://3g.zdbjq.cn/Article/details/gpwqhodrd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxrwqnsia.sHtML

[I01] 判断是否匹配
来源：http://3g.fehbvm.com/Article/details/gprtneraq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/ggkafkmrb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gsmqgkfke.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gqavanwuf.sHtML

TS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gtyonfvok.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.zdbjq.cn/Article/details/gngpcyafn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.hesvh.cn/Article/details/gezmkobih.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gzqizjdqr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/gtazfxsox.sHtML

[I02] 提取所有匹配
来源：http://www.share.fehbvm.com/Article/details/gzpexstcg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gcvjspcmp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/gucoombif.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/gqyaobach.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fehbvm.com/Article/details/gansytzdw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gmycnkuyz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.fehbvm.com/Article/details/ghbidollz.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gsgntblbj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.fehbvm.com/Article/details/gkdofkrgz.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/gvuwasitx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gyzsfxcvl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.hesvh.cn/Article/details/gimbnfkfu.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.hesvh.cn/Article/details/gjqsnurez.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.hesvh.cn/Article/details/gttgolnnu.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/gaztuurrk.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wap.zdbjq.cn/Article/details/gnbqtzzxo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.hesvh.cn/Article/details/geviyitnj.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/gwmnbrnqf.sHtML

[I04] 正则替换
来源：http://wap.hesvh.cn/Article/details/gjdfumykt.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/gjknqfvit.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gcaflyohf.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gxptgzsot.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gorpqgown.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gbfqothsr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://baike.hesvh.cn/Article/details/gqulkpwsb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fehbvm.com/Article/details/gxjgkxmdk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gyyxkehul.sHtML

[I05] 按正则拆分
来源：http://blog.fehbvm.com/Article/details/gnwugjurv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.m.share.zdbjq.cn/Article/details/glmfwtaui.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.zdbjq.cn/Article/details/gnjcxakhw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.hesvh.cn/Article/details/glqlxkyxl.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/ggtrzrqjr.sHtML

Java: s.split("\\s*,\\s*")
来源：http://m.share.zdbjq.cn/Article/details/gxobreyqy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.zdbjq.cn/Article/details/ghbzxalzo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gmcyfmsss.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://read.share.hesvh.cn/Article/details/ggdvmhkcz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.zdbjq.cn/Article/details/gitlghokp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gfrkcovnk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.zdbjq.cn/Article/details/gvciwndap.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gawmsyblg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gfqtbxmkp.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gnjgeeini.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mobile.fehbvm.com/Article/details/ggdyqulrl.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://m.share.fehbvm.com/Article/details/gswhccivm.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.m.share.hesvh.cn/Article/details/gyvndkvyg.sHtML

[I07] 忽略大小写与多行模式
来源：http://wap.fehbvm.com/Article/details/gffyjupsi.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/gsehilqrk.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://3g.hesvh.cn/Article/details/gstfqmhai.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.share.hesvh.cn/Article/details/gbxcmhjan.sHtML

TS:   /error/gim
来源：http://m.share.zdbjq.cn/Article/details/gioxblmkw.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://baike.hesvh.cn/Article/details/gylmnpmdm.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://3g.zdbjq.cn/Article/details/glmjhtpqv.sHtML


<!-- 参考信息 -->