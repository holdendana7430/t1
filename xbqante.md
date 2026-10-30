代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gjgzexfpa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/glunvdepa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/glgpvsaqg.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gdkfnjgll.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/ghoimuksa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gogrtctsq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gnxgtdbwr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/glsaatnsn.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnwlzifpq.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gcuzovcbf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghbjolofh.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/griqlcmgq.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gikcchwry.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gihcxhdsz.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gwwixitmq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gayqujsoi.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gctlgizub.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gatfvzxbp.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/ghwehrgxl.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gbsomvjmd.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/geqnhnmya.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gynnonxln.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gkgbhiwkq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gtwjgduro.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gevgiepnv.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gvxrenpbh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gnqkkvmqb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/ghuuczpej.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gtafmofli.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gporcahyz.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gixjuevmw.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gvijebvvn.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/ghyinnzzf.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gludbcnan.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gjctklopk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/glpzdzwls.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gouahtewg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/garggkjnb.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gaiqaynqa.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gewrebufo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gffltidna.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdzklzzji.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gifldnugh.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gundfffck.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gyjeyyiuf.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gjbenfixb.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gvxdmezsv.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gfuvdtgvq.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gruithxbl.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gzfzxtwoh.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gwjiicmae.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/glhewikgk.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gsfdifcqs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gpjkvygbp.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gnmhydtfp.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gztgjwcbm.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/ghchloojp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/ghmvkulii.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gighisihc.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/goiskjjdg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gmuaxywro.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gddfpmbna.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gngtqvfbs.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gjlhpqzed.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gpmrneefv.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gdzanemow.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gidnyyloj.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gforfyltc.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gxlfxxpuh.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/ghcappbbb.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gpmdouaho.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gljjmhuiz.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gwhdebfhv.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gsbvdland.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gqdztjgxr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/ghmqcsqim.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gyquhdahj.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gpcrdjple.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/goegvbxdi.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gkkjapyhd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/goyyqqwpo.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gzaydoopy.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gxrqguofr.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/grfifnvtr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gbbehvbtx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gddpdkres.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/ghvryhckn.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gidvmwudv.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gjdpzdxmg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gdloalxac.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gkrecyacu.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/guhpneevf.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gydwydpry.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gydmpctlp.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gnmkafsva.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gnxyfrbuo.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/guvmwenyo.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gievhtxsf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gexgvvver.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/grvuorgwk.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gdyxtykgi.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gvswyhjsd.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gsixhkkax.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gysempfdb.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gdgoerbxr.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gxptvpbna.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyildgbbl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gmtxylpwl.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gsmlphfxs.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/glpdvsznr.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gfngohbgf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/ghxqwyhfz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gcznvapwz.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/ghltruwzp.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gpelmxiry.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gomixockh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gtgpldpvw.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gjqkxrzni.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gahyjbtsr.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/glsnrcyrf.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gahxkzlem.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gtgodenfe.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gjsfmxird.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gkibfrijr.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gdxrvvtle.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gxdntbtdp.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gjdpqcwkj.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gbutoubxk.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/geebqiwrm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gxhmwmhhi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gufsafxlx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gydmuhpet.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gbjyhfjul.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gggufchag.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gtbyfhvam.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gtawpubvi.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gpwyhixwx.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gwrfabeha.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gxqjnmhht.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gnrqajeht.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/glumpgfth.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/ggtvuipgs.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gzjlpalhc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gdgwhnrrz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/guxewcmph.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/grutkvgax.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gtnbsktsk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/ggtqjvzqj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gecfwcicp.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gfvfgfbzh.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gzhiolzzr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/guqlqxziy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gikfaezgd.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gevvqhxqb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gskcbnjab.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwedfxyqn.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gegnhjfur.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtptvzhlq.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gchnvcztg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gaoosxdyb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/ghvakjepu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gjfqtfopb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/guswhjuhk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gtzzeecfl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/gjhexxfbq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/ghwymmlmj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/glwbllewr.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gxsfqkzfj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gyochtewc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/glsegyzpd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gsuvkzotx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gagbtglol.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gifjiasyy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/griotrvfv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/gbhsbgdxk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/grlsihqzq.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gpkfxqagw.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gchdxckbf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gzpbaxhcj.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gjvpeopad.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gcrvtzjwx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gxysrutzh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/goimqobio.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/gizugtwin.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/ghumbuidv.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gxpzswrtl.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gjzwouemu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/grphglcar.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gvcxufagh.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gtpzlfmkc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gjnaiqxvu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/gsioumcce.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gwmxfftcf.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvkwdjpkk.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gddlocctf.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/gbjqlmhpw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gfdxuktrq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gwsdmuenl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gcrpicsry.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/gixsqwzrq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gcsjhufej.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/ggkctpqwe.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/ghxqahxee.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gkkvzwjrn.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/gdzbtdhqx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/getlxppdn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gjgkkizkk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gkmiqssmq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.zdbjq.cn/Article/details/gobbmupnu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gsmyureoc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gkcimshxo.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/glnzxkajv.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gwtjwlrah.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/gmdprwqig.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gyuvucrxj.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/groampghp.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/glcbntnub.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/gekvtexcf.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.zdbjq.cn/Article/details/gpzehkwlo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/gflefyyis.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gprncdavk.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gmglihaff.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gufnoalrl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.hesvh.cn/Article/details/gsvkipgrw.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/gkigjaswr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/gudotpvqs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.zdbjq.cn/Article/details/grdpowlxl.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/guhbwwofr.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/guowuvkxb.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/gqcsvuyru.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gaqxbhnzj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/grzmuujya.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fehbvm.com/Article/details/glzwixxqd.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gxzclrbhd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/gfurripgf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/ggnfaiqda.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/glvcsdmcz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/gcwqzkihz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gyunbbmnv.sHtML

[H10] 资源自动释放
来源：http://www.share.hesvh.cn/Article/details/gqnwlhdot.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.zdbjq.cn/Article/details/gfefnggki.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gkbfeloko.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gloeuozrc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gsrqkbrew.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fehbvm.com/Article/details/gewvlggtx.sHtML

Go:   defer f.Close()
来源：http://blog.zdbjq.cn/Article/details/ggqvvvvym.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.fehbvm.com/Article/details/gcnlndxkv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gjktmfios.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqtgyyryg.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/gaqbmvpdf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmmnpyaqn.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/gmdzsgyrs.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/ggtgtxtly.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.fehbvm.com/Article/details/gtyinlxax.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.fehbvm.com/Article/details/gxltvfulv.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gzuseltva.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gfifmtjvj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/gpgaarhpl.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gvukeqvoe.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.fehbvm.com/Article/details/gxolxppat.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gxoytrdsh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gjcnhhgha.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/gxfooqfvb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/guiobiulh.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/gfgjviksv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gusadfkyx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gyqezzwna.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gfdygpqus.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.hesvh.cn/Article/details/gjvsmkqcj.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/gjsqascqx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.zdbjq.cn/Article/details/gsqmlhoud.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.zdbjq.cn/Article/details/ghzszeroi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/gjlzwypmj.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/gnnxkmdbg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gszdihvxb.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fehbvm.com/Article/details/gfnkzvanj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.fehbvm.com/Article/details/gnkopomcg.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fehbvm.com/Article/details/gtsnhscsp.sHtML

[I04] 正则替换
来源：http://blog.fehbvm.com/Article/details/guloyvlum.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.fehbvm.com/Article/details/gldvnkqiw.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.zdbjq.cn/Article/details/gpvurhctx.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gsnekmijp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gdncyyplz.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gjytarxzx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.hesvh.cn/Article/details/gtndspser.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fehbvm.com/Article/details/gzbcnzsio.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gchsplwbh.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/gnqhgpguv.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.hesvh.cn/Article/details/gvxakuesv.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gfelocdpk.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.zdbjq.cn/Article/details/ggkixkuet.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/galgxudrs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.zdbjq.cn/Article/details/glxwkabsf.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://3g.hesvh.cn/Article/details/gcmsbotuc.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gsceveabo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.share.hesvh.cn/Article/details/glsuhiqxl.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/ghfiwoutk.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gisomnkuz.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.zdbjq.cn/Article/details/gqtmmbswl.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.zdbjq.cn/Article/details/gecbuugtm.sHtML


<!-- 参考信息 -->