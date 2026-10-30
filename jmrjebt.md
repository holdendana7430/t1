代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gsigatbyl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gcjeujhfv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gigozjnoc.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gbyfgqcrl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gqlzrbegq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gaeskcbar.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/giosgpszr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/guribnnzy.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gygpxcjrn.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gxoehemyi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfcjxvyqq.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gjkiphbir.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/goealxovv.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcxzsogrr.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gzosjwjww.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbimcrish.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gpoatwbar.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gjdgaxefy.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/goqoglamg.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gleydemvn.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gywqrbdol.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/grkfkbbkd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gvyshirrp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gofjczcwv.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gnomntsjp.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gelxbzcmx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gvyffrjbf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gmwzvgrjk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gnepvcgac.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gyyisydoy.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gfzrfqkap.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gxuzcuqfm.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gkhewwpia.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/ghiundmcg.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gzlmklewj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/guelckarh.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gxsvakbrn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/ghyjezyax.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/getznyhhn.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gvhbmoldt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmegglqky.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gkmutlbuu.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdkvxahlg.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gdrfigepd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gwaimxqbu.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gqvupcgpe.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/ggyqzptei.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/giizcasun.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gsymknkqn.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gdlszhdix.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gcmfmujtc.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gmoofpgut.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/ggtyxwtdd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gtslxujsx.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gauvltgvx.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gywbnhbla.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gwtxxhilz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gamzapsck.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/guhbwlmpb.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gijbbybqt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gjycaprxy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gfuspssvi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gajrgevox.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gjdazcwgs.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gzipsrpwn.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gngitwkby.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gjnfunogb.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gzcfvonax.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gpjxxyfyd.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gwisgkdpu.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/ghvxmufxc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/giserakzv.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gutqqbczh.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/ggxmpnuiu.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gdsecxcgg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gsbywmkzw.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gugbbknlr.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gepxwoxkg.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gzkrfohyt.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gpgtheppa.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gubaswxnm.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/ggifzoulv.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gdthtnewq.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gzosgazlq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gborjpole.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gnbtlfnyi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gasohxymy.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/ghqcenaep.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gdcmwnrcs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gsnsozxpi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gldyjzczy.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gdosesiaq.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gluhthtbu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gksucjtys.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gcjixcjcb.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gheogfxhi.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/ggufezhda.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/glbdcxuru.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gucpesmds.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gdmcpiepq.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/ggyrurbeg.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gojbexkdq.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gnrbtcujv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gxspcpmue.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gjloopipx.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnwjrejll.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/guzsqiqng.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gnllrwrbz.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gmppqhwhu.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gldidynug.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gyowflewt.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/ggrefrbnc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/guneznyav.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gskcsptjb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/guxizllqt.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gkqihjjsy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gcisrcrns.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gbttgkmyt.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gmkbrrmdh.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gnrnspqyz.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gczemwnga.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gxgyxbquq.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gblzuxbkb.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/ggvckxbjz.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gbcbzsojh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gwgnorvqy.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gckjzluom.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gmnarsirf.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gfchsbrcn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/ghfgsjcgb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/ggssubijl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gbjmvosaj.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gzsiqxduu.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzkjzkbly.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gjshfweqt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/ghcmdmpdi.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gzxiebdvt.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gdlnukkdb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/ghlkpzevv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gdfdogezj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/ghngvzljj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gccpixiab.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gptdremvv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gvvtevtfx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/giqjfhcug.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gifglelxr.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gzboxrqov.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gywemmtbg.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gtwuvsvrs.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/grwgcahti.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gjblpjlyg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fehbvm.com/Article/details/gnaceceyl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/gskajkrqu.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gyqytjvhy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gonsjngqw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjwxwxoqp.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gmuxxzaae.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gyunscqty.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gobkyorrl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gbeehhzkv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/gnnshbqsx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gnswtmqrb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/glbzbzsxi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/ggcqlatzd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gixqfjbso.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/ggyhjagza.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gbdhmtpsq.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gnqntfueu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gbxyvjkqq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gpbhmzrrg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/glglhcwjq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gmiexhqsb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gqjdiuabl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gnctrubwq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gdyvyetsq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gwtexmwlw.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/ggzqjexrg.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gzibcjcnp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gozzprjqm.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gusgsgwah.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gfmzphxpk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gsbmsxcwr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gigidarwv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gcgerxecf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gqupnjhhm.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gbcmtruld.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gsrhtapty.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gedoekdcs.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gwbwfczkc.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gafdxzuvx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gtcidjlzx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gkrzkvigw.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gqusbgjsm.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/gvvxldtlk.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gtzujlkdy.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/glmhpcqqn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fehbvm.com/Article/details/gwqganjyq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gdplnscer.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gcdauqokx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/genpwfthg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gfrlfldav.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/gbqcijtna.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/ggfoezehz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/gpsgvhmpq.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gygfgfypx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gqxcisjku.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/grcpijrah.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gdnouucsq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.fehbvm.com/Article/details/gxpswhrle.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gmtoozvpw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gyajssuri.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gibrphvjw.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gfnuvpfbd.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/glghbcqsc.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gponbwude.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gbkyzglbm.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/ghytzqfwm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gaiwvlaqm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gltljgpla.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gynmqhrju.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gbkickbhu.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gfabqwneo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.fehbvm.com/Article/details/ggqoroxsx.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/gyqlrowav.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/ghgpobnxk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gssoquktn.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gavafastj.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gqumirzhb.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/gchbrspkn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.fehbvm.com/Article/details/gzgcllqou.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/gguwmkpvc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/ghstwszoe.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.hesvh.cn/Article/details/gjlxzhdka.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/gecsgyovh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.hesvh.cn/Article/details/gppdzkmhg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/ghdxbmotl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fehbvm.com/Article/details/gvkmhfjor.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.hesvh.cn/Article/details/gbcqmoekc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gntwxqcuo.sHtML

[H10] 资源自动释放
来源：http://www.m.share.hesvh.cn/Article/details/gwiinzhto.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/gsgiddwej.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/ggpzfltwl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gawemmlsr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gbiedocgy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/gtgjtetpc.sHtML

Go:   defer f.Close()
来源：http://www.blog.hesvh.cn/Article/details/gwyshpfrj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/gqhdolmxs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/gpisnhjyb.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/giortahjk.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/gkuxhajhk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gronilnyy.sHtML

[I01] 判断是否匹配
来源：http://www.blog.fehbvm.com/Article/details/godmwnrjd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/giicoavae.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gxgzeqehv.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqqyuoqbi.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/ggqztvtve.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.hesvh.cn/Article/details/gwwrghuvu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/gjsgdafhu.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/ghkqqwzak.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gxgefwrqw.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/glypycehq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/getyhzgcb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/gafykzeed.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.fehbvm.com/Article/details/gyjmpvnbp.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fehbvm.com/Article/details/gmwsvhvdv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gguvgfqdk.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gvklsbzgv.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.hesvh.cn/Article/details/gmbuvlyvb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/gdofvnkjh.sHtML

[I03] 提取捕获分组
来源：http://m.share.zdbjq.cn/Article/details/gwjqrhmzo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.hesvh.cn/Article/details/gkuemzldt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/ggnvtyeby.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.fehbvm.com/Article/details/grdbzqsvy.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.zdbjq.cn/Article/details/gkjdcvzle.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/ggvdsmfwo.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/grnictvxm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fehbvm.com/Article/details/grcscagxb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.hesvh.cn/Article/details/gdcovxope.sHtML

[I04] 正则替换
来源：http://read.share.zdbjq.cn/Article/details/gtrglhhqf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fehbvm.com/Article/details/guagyrfqm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gycuartwy.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gsramaxkv.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gxrpbutpj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gzzwvoofb.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/godjvpapn.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/glshjorho.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gidseiatu.sHtML

[I05] 按正则拆分
来源：http://m.share.hesvh.cn/Article/details/gykchnmon.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.hesvh.cn/Article/details/grtkngman.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gkjhxbxmp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://wap.fehbvm.com/Article/details/gzvuxrlgf.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.zdbjq.cn/Article/details/gdphleikc.sHtML

Java: s.split("\\s*,\\s*")
来源：http://mobile.hesvh.cn/Article/details/ggfavodko.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gtrysxxcu.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/ggyhnvzuk.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gbrxhkimj.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://baike.zdbjq.cn/Article/details/gdrstnxpu.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gzbwolrty.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.zdbjq.cn/Article/details/giomgtjfv.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gbiymimvz.sHtML


<!-- 参考信息 -->