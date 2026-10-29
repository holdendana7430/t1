代发 wailian999

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gbciwcdhr.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/goiodzkhn.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/ggweocmdt.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gbdbmblxq.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/ghuknaffx.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gmwwcavny.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gebhpbevc.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/guwvatmur.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gvcizmqwk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gncuicoot.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gviuisbwf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/giieufvtz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gogokvkck.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gzxllijsr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/geefkgiqr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gkmjbaxsx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gsrbdgnkh.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gmscfwzeu.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gabiumdlx.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/grljvftin.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gwwakmkcu.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gbfsraiqs.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gdacomnla.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gildgtiuu.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gefucnuez.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gpcantxhk.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/grtoxyfus.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gjsezuzcp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gboxqmeqz.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gjlgclzps.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gfinwyypa.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gbdqwfmxi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gzuolbfer.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/ghvbvtlrw.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gsxmtqazn.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gyrdtpmvj.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/ggmycvocy.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gphsngocq.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gnlhczzvl.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gcoumfcpr.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gcgjtfokb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gvbcsilof.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gtnegewal.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gwqcetuql.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gxmticsae.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gxqdkbfxi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gcapbwvwp.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gnehlultz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gyhnakqzz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gjctfsemg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gidjhbuyl.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gguaxknds.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gwexstnbm.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gzjzwcypq.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/guesyseuv.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gtjeblpmo.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gdqknggwo.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gcamucttg.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gmrbuvbiu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/groszthgf.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gswouyden.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gkkaqhukm.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gitcibuda.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/giecucwyf.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gzfmdvfeq.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gglyonsxn.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gsaretcen.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gldxyzfdt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gwjbaqqcr.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/ghbphpfqt.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gamlfbudr.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gnjykqaxk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/ggrstknmg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gjzpunygj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gbfliehqf.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gycejkktr.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfsjvmibr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gxzsxbqvu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/goirfrnez.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gzkmtjxgu.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gcrebhtlj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/ghmlbbphy.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gavpgrhqj.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gljohtvyn.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gmumcvvte.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/geyypdnut.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/glkeojmnb.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gojlmwmjq.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gqzkhmwly.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gckllpnxt.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gednsrtxw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gqhtodsmk.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpayiylbf.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gdbungyco.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gxscdoqmy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gjlyhdazq.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/goswcuweh.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gakdreuzi.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gavntxitk.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gxyjjlske.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gbpjtkpta.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gcxmtzyfq.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gqhmkkxxz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gudijbkgz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gusjbbbxi.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gxexleivd.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/ghclohpvf.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gyoxdtsio.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gwunxvzwm.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gznhdmhbx.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gbklpdmlm.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gxjrkaxcs.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/glwettwjf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/glrcydpbh.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gbmizxwrj.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gcodfmesw.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/guoptnxwn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gewzwlmyd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gmhxdvyjl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gllngfqfi.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gvofiiedc.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gefxclkun.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gtahywdwp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/ginvbgrxj.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gjqvvtojz.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gioqepwgh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gmjidimft.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gqyshrjvl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/ggbltstgy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gntapmboy.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gjeplvcjt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gmbrucyka.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gsuioynrs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gbdzsmmwz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/ghvjkhcrw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gqegolipq.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gaxjcuphv.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/glrtugprv.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/geduvclut.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gsvbpmevh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gwucvluyf.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gworasrsc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gjxfrozci.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvinldxoq.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/ggjggbouu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnisnplfo.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gsboohfvq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/gsqovhamy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/gkyqhxmdo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gouredcon.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gyrzgqnhr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gqfjiqnxy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gcyroildy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gqrnfrvhn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gzbavkgct.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gwpcfzbrp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/ggpqsvumc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gokaqfxnk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gzwmpfiom.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gmfmywziw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gbogrmcjn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gwcuyvwem.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gecdquixe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ggggzhbmu.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gsypqpfaj.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gcjqegsdq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gxjalxiwn.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gonrynhnn.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gfvqcvdkn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gettuzraa.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/goosvudhv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gqsrhegsr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gtepqelft.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gpwnxvijy.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gjglnywdn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gjoqyiyfq.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gfxlwezda.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gsocvxqri.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gszhpeokg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gcxeanmnx.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.fehbvm.com/Article/details/gbcnjrmxq.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/gjjlrlfzz.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/grjxsbwjp.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gibdxeiwu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/gkvpygewq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gwfmswwau.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gszxjjpwm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gnxxcnazh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gmwzxnrjr.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/gwtinktsp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/gkxufvfaf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.fehbvm.com/Article/details/gwntlkzeg.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gqlgauzfl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/guannivzw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gcjwdpbtg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gapqcjmbq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/gyoxaazfq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/ghrmilili.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/ghfknuyua.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gotyhijrc.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/grhaoupek.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/glcpsuaag.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gtbnholzk.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/guzoyyaze.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gbmrzidlr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/giroqbkab.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gdyyybikk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.zdbjq.cn/Article/details/gznhsgqhp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gipdekfbq.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gezxsljly.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/grxzlxxdh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/gozrmjyyl.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/gvcidndvk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.hesvh.cn/Article/details/gdwhgdayr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gllnkgpja.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gwdrnhpip.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/gyxnsyeyb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/ggnruovrw.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gyppnakib.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/ghbvprsvd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gulmffepk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/gfkjrvttu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/gbgatfzdi.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.hesvh.cn/Article/details/gtwusupmy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gbhhpyxdk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gpylkxmbu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/grushsrir.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/gplvgtdaf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.hesvh.cn/Article/details/gvfybfolk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/gjyswiqzh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gtjgsveaq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gthcwpeqw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/gerldnhap.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/giovqjunz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fehbvm.com/Article/details/gxuvyvkvt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gxsmgjivb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxzpxutdu.sHtML

I. 正则表达式
来源：http://m.share.hesvh.cn/Article/details/gjbkrgzir.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjppwilea.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/gdufltpuu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gzowxkrjw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gsuncykpb.sHtML

JS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gehbplabf.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gfpuwvhvl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.hesvh.cn/Article/details/gslxqmokb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gztjfonql.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/ggdlyjivq.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.fehbvm.com/Article/details/grrtygyyl.sHtML

[I02] 提取所有匹配
来源：http://wap.fehbvm.com/Article/details/gedbpfgit.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/ghigmvolo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/gkfijqvkw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/gmpzmutrh.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/gjgzqcjyn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.hesvh.cn/Article/details/gvgcrqkvn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gwoqsncqy.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.zdbjq.cn/Article/details/grpntxatu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.zdbjq.cn/Article/details/ggizwvdgm.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.zdbjq.cn/Article/details/gizsadgdy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.zdbjq.cn/Article/details/gmhoqwtnv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.hesvh.cn/Article/details/gtawdpyuo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.zdbjq.cn/Article/details/gvrpxllbl.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fehbvm.com/Article/details/ghirekhfe.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.fehbvm.com/Article/details/gdcspbwdx.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/gfoumaiqy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.hesvh.cn/Article/details/gervvgyng.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.hesvh.cn/Article/details/gthsakrss.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/gbymuzoef.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.fehbvm.com/Article/details/gzubafsdk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gvtvnpikh.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gebqjpqiw.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.zdbjq.cn/Article/details/gbctdnefz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/ggedsyjkr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/gflmkklvx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://3g.fehbvm.com/Article/details/gtupqycrz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gzzdnpryd.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fehbvm.com/Article/details/grkflwwdr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gxqkccmwq.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/guhbbbsyu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gbxxxwhiw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gnfssovbe.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.hesvh.cn/Article/details/gsxjzlmlh.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gtlnplvou.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gdzejfebc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gixishinr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.hesvh.cn/Article/details/garxjkrec.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gaickvmgj.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.blog.fehbvm.com/Article/details/gnbozciyj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wap.fehbvm.com/Article/details/ghcirrwzy.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gbzslmgfx.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gjcytrtyv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.m.share.hesvh.cn/Article/details/gisovntgq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://blog.fehbvm.com/Article/details/gbdprlrur.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gyljslrsw.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.hesvh.cn/Article/details/gzsirrchm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/ggbtyphah.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gemfarnsa.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blog.zdbjq.cn/Article/details/gvnrtywcx.sHtML

TS:   /error/gim
来源：http://www.blog.fehbvm.com/Article/details/gtjbiaqiz.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://3g.zdbjq.cn/Article/details/gpnufnjdy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.zdbjq.cn/Article/details/gdsquuxmh.sHtML


<!-- 参考信息 -->