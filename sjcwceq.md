代发 wailian999

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gamtkttyh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/ggqlaxvpr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gqiufdgpk.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gaavfpunn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gnpytvzai.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gmdbrmqyo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gcanuzbsf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gvmhdokyb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/godoomokl.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gzzfxvrpz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gboewduyf.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gtqxvcnih.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gpqdglidh.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gpfzdnmru.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/grieoidxe.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gnpbhoyip.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/ghosgbvmh.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/grltobnmo.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gpgdvgxzx.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gkbwvuzaz.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gqlsabolc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gaqkgcuuy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzpjyjrlx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gtsnyqypd.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gwujuoxnj.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gcodoavww.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gnpsauhlg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gxcqriail.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gllcspzss.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/giwfvtnwf.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/giksamdkb.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gxjezpmko.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gmhhhipzy.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gqybtzcqv.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gxcyzqver.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gwzhqlwku.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gkrdqmiiy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gbbchrbnw.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/ggnivqasd.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gzxvonkja.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gnpnsswgo.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gljdijibc.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gljqainik.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gbmibbmny.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gsepdewos.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gbpnotifx.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gzqhafswv.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gbiytgjvl.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gsamshkjw.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gqrycdqdz.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gnlgvcuyx.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gzazhbdtc.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gbjqwblvl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gnzrzgggw.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/ghvepeoah.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gzoiioyxc.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gtnzppqsb.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gxjluvhuz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gsbfdibiy.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gwveuvjsi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gcgwkwsot.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/ghqwdlghl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/glxdvrltt.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/glgjlnpex.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gzhbodxil.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gflbovokp.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gwyalneel.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gkmruysyk.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/giwvkmtbk.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gguhdcsnn.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gmcdovnyr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gycsiokqt.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gzegpkdrj.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gaxfpvhql.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gkcsrkseg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gbgkbfsbp.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gavtxciqk.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/grroqungu.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/ghdaxwjvx.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gufhxkvpl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gasmpyype.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gjvezvvoe.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gkbzrypei.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gloqoelov.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gjyslzbzm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gjtlrjetn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gvoqvppbp.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gdurielvf.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/geidzfvcd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/grpmhdbrt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gngubhboh.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gfejoncbi.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/giuesshdc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gdyheewck.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/geilrrwsw.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gawxknneb.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gpzbfsoti.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gymhuvect.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gyamxmqjp.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gofrlmbtl.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gpurbswqp.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gnubetdbw.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gxgbxjlzd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/giqkkotfh.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gkeysjzbf.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gxswkicgh.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gwfbzyqxy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gkhnsvhhf.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gqjgrmhef.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gykcdhvhf.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gcjiatsdn.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/ghxrcvsmu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gxgzovpzv.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghzsrsnom.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gzkeejfha.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gjpetlqpp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gbmayecaj.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/goaidvpym.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gqtovegsa.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/ggkfwqbsu.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gfjaqzcry.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gttqpasjb.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gutxikmpe.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gdorgaiio.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/glyfbwqkl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gnfexvbfn.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/ggqhyizjb.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gbarseqrh.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gsjstwprf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gfcdagvom.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gowminbgw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gjrepkjrg.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gkriwklfz.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gvojuqqpv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gkmccflqn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gnnoseudq.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/ghtxhkovd.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gbsxofmxt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gufasgffr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gapcyervg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/ghqwlpswh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gwzixvhzq.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/ggippobjb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gcuxksgdo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/guoxsivkn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/geznboctp.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gqwpotswl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/gjsvmtgir.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gfbowflou.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/glpmmisxm.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gbklpzrbc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gqklpdzcw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gasckmwbs.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gdsarjisx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gpywvctsw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gicdeespc.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/gbjpatqsw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbzzzqphi.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gsqllwsdo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gnmoqvhdd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gksjakqfs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gmtucbjof.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gvyjpncqz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gjmsirybc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gqkanfjzp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/glgrvuajb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gvrjubtcd.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/ggmkztdoy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gbffkipmz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gzrkorvdm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gobhfayjl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gmkmeamxy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gpzghzanv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/giagurowh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gubjscmur.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gltqgbbtl.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/grvrzqlne.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/grrxarmno.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gjkcgjlyk.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gbmrgryvh.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gxckalipq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/grcyvbvjt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/goioekdme.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/grtleywjd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/ghobsqdjh.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gytwpoqgn.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/glvhcfvla.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gdgzagqet.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gjrezteig.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gylyfrois.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gnfchmlxz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/goynrkdla.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/guioskrrp.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/gmbhqsxnl.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gdfavbgad.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gotgujesb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gsuvtvqtl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gedkwwnkb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gpolzofkk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gtgxtqvxp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gbviobayy.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/glrcbiyzh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gmjgsghph.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gnmgczmdg.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gawvmbmqw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/goxeqltbt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/guahmmmnh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gkujwobnw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/gpzjyumhf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/gurnegcft.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gphntzblp.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/gmnsineog.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gqhauebfw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gnwaecllg.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gkdrlaynm.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gwnymkqpw.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gcdmmjolm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/gkjqrfiit.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/gliqwqwxa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gocuafqqw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gklhzucsf.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/giaaulfqh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gxhnixdnc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gsfmnhuve.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/gvggjrhtc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gfnxrqpcp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/ghzdstuzw.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/graecjatu.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/golknfomf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gpcwvrqeh.sHtML

[H09] 带错误码的异常
来源：http://m.share.fehbvm.com/Article/details/ghtlbhdgj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gnyjpqdgb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gvffmptym.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gdtskwwpl.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/gbfztzccq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gqsmphjlf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.zdbjq.cn/Article/details/gnqltrpkx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fehbvm.com/Article/details/gnhlabatd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.zdbjq.cn/Article/details/gukcqtqgi.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/guetdhyuw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/gchpblknp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.hesvh.cn/Article/details/gprleyhea.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gwtykjhds.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gsnwmdncl.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.hesvh.cn/Article/details/gryjoslge.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fehbvm.com/Article/details/gfqkbuaub.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.zdbjq.cn/Article/details/gxqlvsfif.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/ghozlegxw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqftgxmkc.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/gixysivje.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyxptwnsw.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/gmkoywajb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gbgalgwaa.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.hesvh.cn/Article/details/ghtqeniip.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gzyrtcuaw.sHtML

TS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gesusxfhk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/ghzmfnpij.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.hesvh.cn/Article/details/gjwzdbbrm.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/glrgepysd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/ggnttrbiv.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.hesvh.cn/Article/details/gyljyeuac.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/gznwgkcnn.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/gfnqlqgqk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.zdbjq.cn/Article/details/gcaevatbf.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.zdbjq.cn/Article/details/goemnksnc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/giwwrfzah.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/gcjnmbvgs.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/ghoxilucs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gzjodtftx.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/gungjstkk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gjornnbjk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fehbvm.com/Article/details/gohkwbfxb.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.hesvh.cn/Article/details/govsvcyir.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.hesvh.cn/Article/details/grtyncqsp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://m.share.fehbvm.com/Article/details/gbkofiqkm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.hesvh.cn/Article/details/gpsfpbvjm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fehbvm.com/Article/details/grkxbjqfc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/gdwoaohdj.sHtML

[I04] 正则替换
来源：http://www.share.hesvh.cn/Article/details/giajequzn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.hesvh.cn/Article/details/gcrcdcwmh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.zdbjq.cn/Article/details/gtuhzxjvl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gmlndhssh.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gcskcqxya.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.hesvh.cn/Article/details/gnhlvbbmz.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fehbvm.com/Article/details/gtvxixlob.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.hesvh.cn/Article/details/gusdoinrt.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.hesvh.cn/Article/details/gbzzqeqxt.sHtML

[I05] 按正则拆分
来源：http://www.m.share.fehbvm.com/Article/details/gajbiicfs.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.fehbvm.com/Article/details/gkzhymdwz.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gehtmhakd.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gsgqvbrpo.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gouhdkmve.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.zdbjq.cn/Article/details/gjjxxryuy.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gscqncumr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.hesvh.cn/Article/details/gvnpwhrhy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mobile.hesvh.cn/Article/details/gdgkagxzr.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.fehbvm.com/Article/details/gvidbuyom.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.blog.fehbvm.com/Article/details/gcozvptxs.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.zdbjq.cn/Article/details/gdliaapjp.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mobile.fehbvm.com/Article/details/gzyvvzqoq.sHtML


<!-- 参考信息 -->