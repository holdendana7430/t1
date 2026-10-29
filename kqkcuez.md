代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gfmjrhtfz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/ggvmktdfg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gswdjvcvs.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gkgtikofu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gplwtcuup.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gjrkbptwr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/grjuufgrm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gvevvlwtf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggthykxkm.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/guuqoddxk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gniqsqlpo.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gfubpcsrx.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gjndhtixh.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gvqwwxvhh.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gwxvvvcjj.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gmxjwbjgr.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gpddycbki.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/ghykzncio.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gffgowakf.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/grcrcfokh.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gbvenmchz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gbpkukhjv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gohgfsscr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbozjllad.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/grszgjzqk.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gavpdgafb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gfeedrucq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gxlnvoenw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/goahgzhig.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gggmjqoax.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gwxgcsiqi.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gfoaqtvsx.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gpqevmhol.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gulakukei.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gpfwaaveb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gchzinmec.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gurnacuht.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gmodnvgti.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gybwwmxpz.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/ghwmywhid.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gjmbkukft.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gejnrokak.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/givgarvua.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/ggaqflevh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gfsxjzgro.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gckrkkuxw.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gyrgbxlem.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gwcuxionr.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gnjvkyskm.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/geqvfneqa.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gnlfmiwrw.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gwcdjblah.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gbgkjjfhv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gteivpkhn.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gdfljboxy.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gkizbzioi.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gooqunyaw.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gqxeldynf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gagtwphwa.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/geaaoutlf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/giaazmuuz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gsoftdysu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/ggldpxuzf.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gyjetrlsx.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gfapmiuak.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gqrhvoiqm.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gmpjgehaj.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gwlnbtfhz.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gijfnvthj.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/ghnwztiem.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gwrwahrog.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gwddibntx.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/giwmixfws.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gptnszels.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/ggpjdbmzr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gxjctlwvx.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gehkkojnc.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gqwaqbebs.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gczyikeov.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gttmveppi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gjjnrlmqt.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gupcuuxde.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/ggpscwecg.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gyjthpgpm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gedbrenok.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gdhghghme.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gpadiptqh.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gxaaacfst.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gdtdgloav.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gelilxfvr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/ghagzmqkn.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gvbmrnsui.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/glhqiijga.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gxxtxzddf.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gcgddzspo.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/grexcdttl.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gtvnrqrrz.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gouunasbf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gtmfjguev.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gfukmqbmg.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gkymozcgr.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gdpuggcfe.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gwvmmizyg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gynymvwqs.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gfriyigqk.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gnkyfched.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gdnostinq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/ggpdartji.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/grmpqkdnz.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gosqidgyx.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gxiluxequ.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gemivixgu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gdwflvarr.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gvcltdqzh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gmzhnhkjd.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/guwmkzvto.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gteyotkxu.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gadrtvdfw.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/ghxufamfw.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gzxvbjmxd.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/glauaawiz.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gienrimeq.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gmatnhbex.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/goznfrmmq.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gmmoiyqsg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gialjndmn.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gdiyqmugv.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gjmxkcwfp.sHtML

[G14] 数据类 / record
来源：http://blog.hesvh.cn/Article/details/giaiekgfk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/guiamqvti.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gvhpjpvdy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/ghaibhgee.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gwjcarxmy.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gkebsotca.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/grkqshtak.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gzpwrjezz.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gzekzuirt.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/guzjqdlvq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gtvgjyvrx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/ghstszbiy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/guwhjsaeh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gnngsvxlk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gejlzztoa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/ggoxfghod.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gpzznwcmn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gipvytmlt.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/grfykogrq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gofmdjrnm.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gqpggfynx.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/geaivaihl.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/ghnnlsfau.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gqffmkbwq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gonivpamd.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gqbezzeun.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gfxnyvvtb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtwhrccud.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gwuueyfrt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghlcmgxhi.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gxjeczbmb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gwnrjfwmw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gkxhlklnu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/givrdbixd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gzteedtvj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gubsjmkhm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gzpkatclj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gvljnmtgb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/gwedvesfn.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gydzqvacz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gxdhrfybi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvefruiud.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gizumygbw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/getzywwqc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gnmgstuwl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gkdixcrqr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gnzkqhstj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/guqnzbnyy.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/giasrllha.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/ghikkfisw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gqfiqxbtu.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gesvlshpz.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gteoxkgbz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gushfocvg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/girygrieq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/gweoczbrn.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gmtclcsre.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gpvjsrlht.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gkxzxghdw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/ggxadrwih.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/guncruprw.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gkisodytz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gehlbantl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gkpxwtntv.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gxdhpkkxj.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/gpdzjiznq.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gkcialgqz.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gnfphtxsc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gvmthbtnk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/ghjorkddl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnghcufim.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gmozticsc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gzhyclylu.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gpkrnizdt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gqbzubxng.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/ggpsdydyp.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gbdhpuobp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/grhfhcaha.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/glftwluqv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gtccxbzkn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gbzvkuyfu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gelhhhgdj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.hesvh.cn/Article/details/ghyvvbzvq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/ghypxveob.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gnopgfvqk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gmhuibtig.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/gaognqjfn.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gwcvwyznw.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gebysexam.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/gfplwbipx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/ggnexouyb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/gybrttftm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/girmpubzx.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/gjjfwhxiw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/garjftfcb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/gipzhilbg.sHtML

JS:   e.message;  e.stack
来源：http://wap.fehbvm.com/Article/details/glbudodtb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/gvvtqejph.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/gverdcvup.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gnblbrxci.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/grsszjopp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gzesdocct.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gmtowdeea.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/gwphbpcyh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.zdbjq.cn/Article/details/gjotynanw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.zdbjq.cn/Article/details/goufeyalp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gujwnfcxj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/gklqswoxg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gyxkcwzrz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.fehbvm.com/Article/details/gwrtcdvxj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.zdbjq.cn/Article/details/gfzgfeqof.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/gckhuvaac.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gyftylhzh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.hesvh.cn/Article/details/gwnyiqgsc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gwdbaxqqm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gaaizfhmu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.zdbjq.cn/Article/details/guawxtneb.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/gyjkoelvb.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gtffdlvth.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gohattrje.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfaolhcox.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/gucrdfgpp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gonmxmqzx.sHtML

[I01] 判断是否匹配
来源：http://m.share.hesvh.cn/Article/details/gkdrtxgii.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gwcfoikaa.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.zdbjq.cn/Article/details/ghzzxlayv.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gtjydemas.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/ggsceback.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.zdbjq.cn/Article/details/gdrogbiuk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/gvlqchews.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gjhjyfelh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/gdtixoaxm.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/gexgqexzj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/galygvnuc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/glojpktun.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/grdnfzrag.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fehbvm.com/Article/details/gzywfwhnv.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/goxtypneo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/gjcefjhsx.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gpavvcoyx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gwbqoryuc.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/guqdprqsv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fehbvm.com/Article/details/gditvwrli.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.zdbjq.cn/Article/details/gqpcftybj.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/gleohdfds.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://read.share.hesvh.cn/Article/details/gruhpxlho.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gigacfhgt.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fehbvm.com/Article/details/givvqpyoe.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fehbvm.com/Article/details/gbfxxxlbx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/gbkjhtgvk.sHtML

[I04] 正则替换
来源：http://blog.zdbjq.cn/Article/details/ghaxytslp.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.zdbjq.cn/Article/details/ggwgorluu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gejpuocxj.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gqzmyabfe.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.fehbvm.com/Article/details/gtqggkvdq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gmlcwmnna.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.zdbjq.cn/Article/details/ghzaacyvv.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/gxxyzvset.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gwewaxypb.sHtML

[I05] 按正则拆分
来源：http://www.blog.hesvh.cn/Article/details/glhpntlzh.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fehbvm.com/Article/details/gpycublql.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.hesvh.cn/Article/details/gqjjnykfa.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gsvtfmpua.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gmwovokqu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gmekvtxvw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gkkflslng.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gnuemlyiu.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.hesvh.cn/Article/details/gdyvdlhqx.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.fehbvm.com/Article/details/gmaogsgbd.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.zdbjq.cn/Article/details/gdmmzhjev.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://m.share.hesvh.cn/Article/details/gmffdvfyo.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.zdbjq.cn/Article/details/ghjapovhi.sHtML


<!-- 参考信息 -->