代发 wailian999

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gxqrtywdd.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gesvmhgmr.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gqbgsiovi.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/greofbtpk.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gxqeenhlw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gluuzlyry.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnovsuixu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gzjydnxqf.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gvdzrogon.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/girmkrhdi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/ghgvwaeox.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/govbowtte.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gofaxvtnv.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gptbldotg.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gqbyjxhvj.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/glxwrttbi.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gphbhsoec.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gnjydthfc.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gnwyzagwq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gpxcszzic.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/guqwcnfuy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gldgabkxz.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gevhudsqg.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/getzmfaqw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsugdaxox.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gctnmxmuw.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/grwdgewbu.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdbwbewbf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gyabktmbx.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gwxmaqudy.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gaxpsyvva.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gtmrymprv.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gxnhacpup.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gguhpchkd.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gwvwpdazz.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gflncnzkd.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gbukvubwi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/graudifhm.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gtnghhunm.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/ghixqpzdl.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/grwzxmqfk.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gofurjwjb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gfetdbxvv.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gmjhngcey.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gqkgcmuoj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gmeqpakut.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gyqutftae.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gnlxqmkum.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/ggukbrhwm.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/grjqizhul.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gvciheter.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gezcuoyko.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gtradfeok.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gllzvyibc.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gkylrzwvd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gtsyjwtxp.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gactaxlce.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gdymdnvmi.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gsrgpgucu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gsvpehxcx.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gbcslkshm.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gqidfrdkd.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmdiavxfs.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gorqjepvh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gtjkikymq.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/geolzwkbk.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gbcwxconu.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gsnvpbrnr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gnpnydgfk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gyvaheqrs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gcuddgijx.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/giexeaxvw.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gyyxgxvph.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gehgwsngw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gngsfpryt.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gvdvkyxbs.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gnwhcdfuf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gcwqnxpmb.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gehhxdfpb.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gvepkhtdc.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/grsefworg.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gzztncpyu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/glfjtwbxx.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gcsstdwvc.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gkjaqzoau.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/glezfnqdo.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gxfxkahxt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gsohdxuha.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gcphxcrtd.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gpbsuszou.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/goxapvepr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/girtwvrea.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gtvpmlvhz.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gwpatmrpj.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gezutzzpz.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gqfhudvht.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gbsytymzz.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/golszucsu.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gwwivzyak.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/ggaowgewx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gwfhamdfk.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gkajdzljh.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gaafgncib.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gdioqwusw.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gsxrkfkcc.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gjiknnxgl.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/ghlxgcsgm.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gkccktriw.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gucvfbite.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gkgjrnltw.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/ghadrvrrg.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/glabgvsnx.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gurcswsav.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/grsgfekrv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/grqxjhmmg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gaoeqbqct.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gnuancafa.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gkvxlkmdn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gpafzivpk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gfllxamhv.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gelxwypdi.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gwzxvpdlq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gggdkpjdn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/galrugjnq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gvixpoeta.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gmtkjfqjk.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/giewzewhl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gywtumozs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gnmxbsequ.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/geogynbal.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/gdwzcvsuz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gfygxnwjq.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gaiakvnfy.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gyazweizl.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gtnqumdqq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/ggbntadsy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/glvxfseiq.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gievwfheu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gjlgmuxkx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdkditcix.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/giezmoyub.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbcpojenj.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gdouiehhu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gsggoyahl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gwqdqelyf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gcouabvuk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gpkvsypbe.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gnwnnoxwo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gygqhfsnj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gbraqjhfh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gnxmkvapp.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gemwlskzo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/ghnslzbkl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gfwdqptnj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/ggnnxltqa.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/giijdlyua.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gbbafgxyh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gcdlhmngu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.hesvh.cn/Article/details/ggrtvrlyc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjxruxfmz.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/globjbbif.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gnqcnwgbw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gvhsfypvm.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gihtwebdu.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gbozfpozp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gkunjzfla.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gommlmbyy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gevxlbwtk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gryejclcg.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/godevqilx.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gxcwdvljm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gplwmrqju.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gysxegymo.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/ggnwrqeth.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gqcdlovwa.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gxjdntvrv.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gckvaozza.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gceqgfzqy.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gvjclilew.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gwrlvnwza.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gjjhbvxio.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/givqinpyi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gbbuueuyw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gfzrohqfo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/gbjwnduqx.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gokpomotk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmegymknq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gzfskdaza.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/gmyftseps.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/ghgkzzqsc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gzxmxcjrq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gtrzxnldz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/glanwkxtx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gpsgdunwy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gvxacwxpf.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.zdbjq.cn/Article/details/gacwxzijr.sHtML

[H07] 断言
来源：http://3g.hesvh.cn/Article/details/gaxfufrtx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/gghbaqlye.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gsppyqqfq.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gqcfmlyfc.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/ghnlmybwy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gylmgupck.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gwtoduksx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/ghigujcwo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gusepblyw.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/gyqpifzfn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gveqbasne.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/gxizyailw.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/glrjahqim.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gxtcmuevh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fehbvm.com/Article/details/gckuqubrh.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gdsolxalg.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/goezffgyg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/gwpghunqz.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gzzjtrsvw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gejsofsac.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gvudwgzxn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.zdbjq.cn/Article/details/ghhvrndnd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.zdbjq.cn/Article/details/gehagjyrf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/gynxuouaq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gahwwfgoq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/gjjospsqz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/gyyefyqeu.sHtML

[H10] 资源自动释放
来源：http://blog.hesvh.cn/Article/details/gqshrhukf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.hesvh.cn/Article/details/gxoueaibx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gmydvhnzd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/ghkqtajbw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gpqadyzje.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gwmjlabhg.sHtML

Go:   defer f.Close()
来源：http://www.blog.hesvh.cn/Article/details/gptcefodo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/ghzhhopov.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gammotqib.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfczqazqs.sHtML

I. 正则表达式
来源：http://www.blog.fehbvm.com/Article/details/gxxkblhyp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grrxhkrry.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/gwepgqrgn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/guurqzlkx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/guzsjsyft.sHtML

JS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gqkkkoedx.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gjblmeugc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/geeholzai.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/gmfydwljj.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gztdqshij.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.hesvh.cn/Article/details/giiyqljzr.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/geiufxkmp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gszhzrech.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/gspqvktbd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/gpldybgti.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.zdbjq.cn/Article/details/gewzemfza.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.zdbjq.cn/Article/details/gbzdbbufy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.hesvh.cn/Article/details/gohnlmijz.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gtcogahlj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fehbvm.com/Article/details/gdxqgiabd.sHtML

[I03] 提取捕获分组
来源：http://read.share.fehbvm.com/Article/details/gzawgfnmq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.hesvh.cn/Article/details/gwcfygiov.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/grempuist.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.hesvh.cn/Article/details/gloyzvfeu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gcqmmtsyq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gegeinkgt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.hesvh.cn/Article/details/gulrwbviu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.hesvh.cn/Article/details/gtikrnjbb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/gndnozvmr.sHtML

[I04] 正则替换
来源：http://m.share.fehbvm.com/Article/details/gwzfhrpqi.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gpmsaxuml.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gfiwzqhmd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gihwzuaeu.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gttutmshs.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.zdbjq.cn/Article/details/gdpdqumph.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.zdbjq.cn/Article/details/gzkzvizor.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://read.share.zdbjq.cn/Article/details/gcisrgtrp.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gqmmujncs.sHtML

[I05] 按正则拆分
来源：http://www.share.fehbvm.com/Article/details/gbexuoyhe.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.zdbjq.cn/Article/details/gzczxownn.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gqcctagby.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gbycjurxf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gzeyskend.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.zdbjq.cn/Article/details/gyyanhuww.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.share.zdbjq.cn/Article/details/gycsknquh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.hesvh.cn/Article/details/gzkuyweci.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/gzldlshlm.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.blog.hesvh.cn/Article/details/gpnwihaxa.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.m.share.fehbvm.com/Article/details/gvimuowzc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.zdbjq.cn/Article/details/gmhyfglhg.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.hesvh.cn/Article/details/gzlhtawbp.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gsnyivzwf.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/gceobgiud.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.zdbjq.cn/Article/details/gcwcsotwj.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fehbvm.com/Article/details/gmlradwiq.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://read.share.hesvh.cn/Article/details/gxecqlivg.sHtML

[I07] 忽略大小写与多行模式
来源：http://m.share.fehbvm.com/Article/details/gqjqtklmr.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.zdbjq.cn/Article/details/gpxhuuiaq.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/gmiebygux.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.hesvh.cn/Article/details/gugoshucf.sHtML

TS:   /error/gim
来源：http://m.share.hesvh.cn/Article/details/gxotnvbxg.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://m.share.hesvh.cn/Article/details/gyfxohdou.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wap.zdbjq.cn/Article/details/gfcfvbbtc.sHtML

Ruby: s.scan(/error/i)
来源：http://blog.zdbjq.cn/Article/details/gnqkbmgce.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.zdbjq.cn/Article/details/gveyhndne.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://3g.hesvh.cn/Article/details/gpokouzfg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://read.share.fehbvm.com/Article/details/gdlgmhhbo.sHtML


<!-- 参考信息 -->