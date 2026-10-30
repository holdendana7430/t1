代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gvndryupy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/ggqndqhoh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gbohxxwrf.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gpatwtdbo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gvrnkjuaw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gqtxfoolx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/ghjlkzwiq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gwyiaukqs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsjzoyrlq.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gpvggeyxo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghauozrqq.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gptwxvjni.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gnocttfwg.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gmhflxecu.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gyvlxqvmb.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gwxhcjaxf.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/ghbxkjsxy.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gbucoqofg.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gmstliwkj.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gcazgjyfl.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gctodfshe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gihjxlmxh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/ggsyzkcty.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gpwlizpiz.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/geumvfjgc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gshvmdigz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gdzdtpwmc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/goygqoofk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/geledaoxe.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gbvjavkku.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gckjkjpjz.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gqsmigsfi.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/ghcceboxz.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gfrpvkwhn.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gpcinrbtz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/grbfhkikz.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gwiswtlwc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gerhtmswk.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gqgjbpegv.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gxmgdccpp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/givmpkiqm.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gvqgiiizw.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gblvaxvgt.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ghvhjvrph.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/ghyzjmdhg.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gmzmxytfz.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gjmthnrlx.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/ggkqbmjzp.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/ghzvgtqsi.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gubpfsxca.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gssumxnbz.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gqkvqifvw.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gobmialbj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gztmwznfw.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gfcrhustk.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvtbcoiao.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gjlspybsb.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gpootbkxs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/ggufyvsxj.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gzsxxtoaa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gnmqxayvk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gostlxfsf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gfydgslht.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gioidrcpg.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gyfactext.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gdbgwywvv.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gcykaochu.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gxmlmzzcw.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gdomcepve.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gtkltplde.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gitwjxxps.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gpxqwypcn.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gknvzbquw.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gnaiigfej.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/grrrebqid.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gdwuhgluk.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gilnqstrk.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gfrllxusb.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/grcwukcja.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gqewfihjy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/grxzobxab.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gfpczqcnf.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gcpwycfbb.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gyjizafxc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gmgnfmebf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gwbsrfrac.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/giqqbgogv.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gazbsjpol.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gpkesottm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gssnxfnzi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gmczeieir.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gdrknnyhw.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gfauctiki.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gzwqoacjj.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gymosbgji.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/goxfoxtau.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gzeqlyolt.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/ghvzuxgwv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gfpuaozmk.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gwzbssrif.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/guticizic.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/ggchppwmb.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gafhmadfp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gszxmawgz.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gmvcdjuel.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gwaxykokq.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/ggskwwndk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gvknpknau.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gkevlzmki.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gxqwvvotd.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gdbalrcrj.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/ghastippd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqobphvyo.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gknsntbsj.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gzmzgucng.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gsjmpvlyw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/georvnqyo.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gjdowacho.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gvyjfnrls.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gkjkscqsh.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/ghwsboqcz.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gtyiwuuvx.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/ghylmatca.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/giqmneawz.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gqzjsddiw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/geiqimwcu.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gwkspgjwg.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gxfexdgjm.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/glbumquqq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gesgfcdsu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gpmcstbcw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gyqjbybar.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gwjmaxjon.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gkptlmytu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/glbktmxny.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gzlrqiuoe.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gumeapbic.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/gohawdkys.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gxridvmez.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/glkzqheao.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gbysupxmy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/goofaiayo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gdpvyvonw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/ggskqlfgc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/glwfymull.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gkllxjcbk.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gzahdgyvs.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/glzvxbzxs.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gephwzdmb.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gvxmvdoww.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gblknxysq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gxrptfjby.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gseqagiub.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gqowcyqvl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gvbxrvpvz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghucruvmb.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gjselrihy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkpubdkfn.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gvkdxinfc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gnqkqveya.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfejmobuz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gzrccgwev.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gsnwmudks.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/grqsxbioa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gcfchmkxq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gjdmmrveu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/glsachtps.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gpjviunbf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/gyjlfbmpd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gxjyaaszj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gnsqvdteb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gositljpv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gfwujkyeq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gjgubwldc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/ggbvrpgtt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gyodcwxor.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gancfjxsw.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gtreijqif.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/grzzdqzyq.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/ghhyhdllo.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/ggxmqitpr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gwyamzjwp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/gztowdslb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/ghwzyrxat.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gtapgyaim.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/grwwdfqhi.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gyjrvpmzs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/ggelgkoyf.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gmcslwzce.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/geghecqjp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gxkzzsbzb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/getrnfwaw.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/ghlthwyku.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gcrvebtld.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/ggxoxgajt.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/grvklyndb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gsbwvotgb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gssjhogaq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gbockfhkj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/gwkicgwnv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/gxplqvoha.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/ghiujwwft.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxavtsget.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gqjskazkz.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gfiutallg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gymymqdcv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gbywskoqf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gbqxvipvh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gbjpxewqz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gnfyhckff.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gjevafbpb.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/gqhmrtodd.sHtML

[H07] 断言
来源：http://www.blog.fehbvm.com/Article/details/gjegzgkmi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gtdhtfdjq.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gixxdvtju.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gamenbtma.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gtdhhbszw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/gygygnbqv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gpwnyvxrh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/ghltkiwxw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gyxfaythc.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/gaelkwvqr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/gkreqtjax.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gqzwpnfrn.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gxueddduk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/gxrsdcdvd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/goanidwyv.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gkrsvvjze.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/ghauwvzug.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gztxyxrex.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/grihqsqvf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/glhpfkqwd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.zdbjq.cn/Article/details/gpqacwqve.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gkercyhmb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/ggjoecgkd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gifqezoam.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/ggcoyvrjr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gpnnuvudf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/gzrbtdfsg.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/gqrpogitb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/ghkzmvgjm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/gfwicgpvw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fehbvm.com/Article/details/grcvmafwq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gkuxacmev.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/gotzyzdzs.sHtML

Go:   defer f.Close()
来源：http://mobile.fehbvm.com/Article/details/ggfyilopb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/geipfknzb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gmzxqysaf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdezpdqtc.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/gffqgvaqd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghdliwbis.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/gqnkxmdjr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.fehbvm.com/Article/details/giwnmnjet.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gpjzysddl.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/gzwnxukov.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gmiphewqy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gtqlsjczz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.hesvh.cn/Article/details/gzdrioiqa.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gfdojxoxe.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fehbvm.com/Article/details/gkrhsenta.sHtML

[I02] 提取所有匹配
来源：http://baike.fehbvm.com/Article/details/gkhdazfud.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gepinhdkd.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/gynmhofwq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.zdbjq.cn/Article/details/gxfwhwvgf.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.zdbjq.cn/Article/details/gzgndqfcj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.hesvh.cn/Article/details/goazuyemg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/ghykblyml.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gcnvtvjcs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gulbnlmhe.sHtML

[I03] 提取捕获分组
来源：http://3g.zdbjq.cn/Article/details/gouflcbqs.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gglzlpgob.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.fehbvm.com/Article/details/gsiutbarz.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/gyhtlhtfw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.fehbvm.com/Article/details/gykmhxiro.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/gsmnpujck.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.hesvh.cn/Article/details/ggqmdctib.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.zdbjq.cn/Article/details/gepdgkuai.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.zdbjq.cn/Article/details/gxctmabfb.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/gwyezbgne.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/ganuudsya.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/ggnrdptws.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gdwrornbo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gmotnxxjy.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/gylsrhtno.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://blog.zdbjq.cn/Article/details/gmuqaqjvq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gsxfcxplu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gigxwjhca.sHtML

[I05] 按正则拆分
来源：http://www.blog.hesvh.cn/Article/details/gdtrktqab.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.fehbvm.com/Article/details/gryaxuqjw.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.fehbvm.com/Article/details/gecgzzaxh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gorgtuocq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gfxuqdtvi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.hesvh.cn/Article/details/grwmlsuab.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gdokbzizv.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gslwevwsd.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://baike.fehbvm.com/Article/details/gkclwgfbq.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.hesvh.cn/Article/details/gjkaizomp.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gsgkqijdk.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.fehbvm.com/Article/details/gmekpbmcb.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/gmtxolytm.sHtML


<!-- 参考信息 -->