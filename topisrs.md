代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/ggwofptnp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gbkobatnr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/graorfowe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gtoiuotnn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/goylgbzva.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gqxvtqcrr.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfaainvbx.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gfyxwpxtf.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gnmaifczq.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gssndffnq.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gfpbdjybp.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gsgrkpfrb.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gjypfmoqr.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gezcjpzxf.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gxubbrvse.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gkrcjnpvg.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gzpdzmsuf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gjgvkxbcb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmsojraeb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gkxhldgnw.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gzlnxlycg.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gpqudqqwx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gzzqoxhgr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/glnkehpxi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gzmilymcz.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gmrszhcxa.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gbhfbygbi.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gwpkzceqc.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gfnqnplii.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gwpcwunlq.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gqjemjdfd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gwtunneux.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gwtcujive.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gypjegbyf.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gnaxgeejj.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gxcwqchle.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gkvxbilwh.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gzotbsgog.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gflbthvor.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gifhlelzv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gczgyomuo.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gpbyglxud.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gifncikab.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gbyfxkkwr.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gmlosnnto.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gsfdzorzl.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/grejgeqwg.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gsskzmepe.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gkjhtvcqe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gumyxruzw.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gxalsnewo.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gfyrxqnkc.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gzlvekcmv.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gbyvpjdsn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gwcuixjpm.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gmjjutvoe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gzftkmdql.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gppdeotbw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gsdiilqlz.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gfcwsndnk.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/guuikiafn.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gvjcuizqm.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gixjgfgkh.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gdgqfwcue.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gskglxlhw.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/grzigmvid.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gsqnpofdh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/giqjechco.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gqiteduno.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gskyfcqyg.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gglfwvcuh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gatubthkd.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gvzuqxhdv.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gpufeepaj.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gavsfggzs.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gaiyebyei.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gfcxrqlkj.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gnrwlnvqw.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gmupnccxe.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gjqhwqrwu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gxfcsukvp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gkypvvmnz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gddeutkfa.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gurutoxmb.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gompynasr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gaettujhc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gmicupbql.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gazljbbfm.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gucuqxbos.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gjxxfsgvf.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gzsjogjwn.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gepzztusx.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/glbgktakn.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gqzkksgyl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gymcqvccn.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gxdrviecl.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gtdvxjetd.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gwgecpyjt.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gxrsyzzlz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gzuatenup.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gnpweykmm.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/ggrlaifwu.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/geppyqvah.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gzurcckam.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gljzzpxim.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/goybworxk.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gvhgfbngn.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gstmikvwl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gvjtmkalt.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/grsyrbshk.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gesyqfbhm.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gupljumvb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/geqlczsfe.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gmyysuhsv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gfxwnboap.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gupfsclrw.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gqxzadnql.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/guautorid.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/grgobaooe.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gkjrrdtnl.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/getqnuunb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gxffqoknv.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gfvafswwx.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gcyajhyfs.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gnnrdpkux.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gsbjrvcuh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/glaluytax.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gzxdsdhba.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gjcmyeuat.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/glotuyrjh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gtnqggtis.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/gauzftelr.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gqssxnjez.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gisargoce.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gxdmbknza.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/gfxfdfhwf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/grrttybit.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gdfttvonv.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gnwgrhlqk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gttyauvfn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gscsxfpcn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gkylsjmuv.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/ggtxgbkur.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gybyeohoe.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/ghqgyoywh.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gaujdhjxz.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ggodtofwe.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/gimvxofdx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gxjivdtqk.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gnoggbrdv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gkqnxfgzq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqjjinrle.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gthcrcbrd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxpxipjyu.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/grckoomxf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/gvzkzchde.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gwattwyww.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/grlikjjgz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gjexjtkdt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gcluogoqr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/ghelbfupu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gdswciwbd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gkisgujhp.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gqltttqrz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/ggzstavaa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gofdahjwe.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkatsyyoh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gqgtqncks.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gmosijsnt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gycgtkwce.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/goiszayco.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gernqjhnu.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gvoazfzlt.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gryzjfsnt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gfxhviiyi.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/guloincwj.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/grvsbcrfj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/goxlmlhts.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gbfcquntk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/gnendyywb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gtgmyzavg.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gdjddanwq.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/goriiblyh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/geeojyeoc.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/ghxwvfaxv.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gihaclitx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gnylxgudf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gkaiuhyph.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gjsbivqxf.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gzmnurnkh.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gwacvlqtb.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gvjthprrk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gzmzhyrww.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gzovfbmoq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gifirvryk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/grpbuabpa.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/goziiihud.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gprqveapk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gwcxzjlck.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gzactsuqp.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gdidtgpox.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/ghoofubjk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gtnebhwnw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gnggmpynr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gfdmvfwfv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gehgodczt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/gwbueufxe.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gpxeaqxjx.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/gbuwxokda.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gmnkzpvzw.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gtibkyaga.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gpiexorem.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/guhwfxpiv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/gkrfqospa.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gvvagrmzj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/gwnhawsbj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/goootkmcq.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/gvtbvdmeu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gwmrzfbtq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gxbumhsfh.sHtML

JS:   e.message;  e.stack
来源：http://mobile.hesvh.cn/Article/details/gxdriqxxv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gkkjhwkha.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gtanqirce.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/gyntofpxn.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/gtuxeqotu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/gofhpgsim.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gmtmzydii.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gqtumhoem.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gkqwbdpwi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gryejdpaf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.zdbjq.cn/Article/details/glomhrwog.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/guctdvmmx.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gahdsfijz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/ghkfflzmv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/giiwvpbwt.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/ghzedfqna.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gzulqpmjh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/gtfssxfsl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gfymufrqs.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.hesvh.cn/Article/details/gsfujgwtv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/gfrrqlidv.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/gxkbhhpva.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gwgnykymt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gmnoomxhs.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbybnyhhl.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/gqmiypktb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gofvyiior.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/gwjsirrje.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gjxnqnrln.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/gxfdlkmoc.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gkerqrxrc.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gknbrgezm.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.fehbvm.com/Article/details/gahtlwfcg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/gqnfmircs.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gsgxwswgj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.hesvh.cn/Article/details/gqejxismr.sHtML

[I02] 提取所有匹配
来源：http://www.share.hesvh.cn/Article/details/grqxegbfk.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gpbzavukd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gxyyekdcn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.fehbvm.com/Article/details/gbxwklizs.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/gfzzqgqaq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gccvnmmba.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gueuqxesx.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gobdxnnql.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gvnisbnue.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/gcnxqdrxs.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.zdbjq.cn/Article/details/gzsfvtzhl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/gozyzmmqs.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.fehbvm.com/Article/details/gedmttygo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.zdbjq.cn/Article/details/grqkwqrjx.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gjhzryqcq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/gmqnwtuox.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gilptrvoa.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.zdbjq.cn/Article/details/gxytkaxzt.sHtML

[I04] 正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gelrqqvwh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/ghkxbbtak.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gsihvaajw.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gzlyidmge.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/gvcwpffmk.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gwnlegceh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.hesvh.cn/Article/details/gqqgrqkxz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.hesvh.cn/Article/details/gnqzdokrd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gbvcqmdpk.sHtML

[I05] 按正则拆分
来源：http://3g.hesvh.cn/Article/details/gistmtrvz.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gbvcibxtz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.hesvh.cn/Article/details/glqeraniy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gjmksacbj.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gncsnxhwt.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gnjwzsgjd.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fehbvm.com/Article/details/gxywpsage.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gngjubvmb.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.fehbvm.com/Article/details/gvoxmnzxh.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://3g.fehbvm.com/Article/details/gbvqlcphn.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/guggoyvkw.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.hesvh.cn/Article/details/gadvgvttn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.blog.fehbvm.com/Article/details/gamcdavoi.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gqofadkoe.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gacjcwoxt.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://baike.zdbjq.cn/Article/details/gjpmqedzu.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://baike.hesvh.cn/Article/details/gircvteib.sHtML


<!-- 参考信息 -->