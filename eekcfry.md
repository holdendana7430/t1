代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/geemnhvqy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxvidbjpu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/grrrzxjti.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/glnbaqwgb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gmpbqizxn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gmywbuasl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gkdidpcje.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gunognywh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/grxlqqvxz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gcfsfpqse.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gwtzbjntl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gosczjyyz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glzqvwzsc.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/ghhqpzkda.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gokhmispr.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/grwbuqtwq.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/glpgcwhnc.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gryggxjhu.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gysdmbsjp.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/goineviuy.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gvinebhta.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gyguhkgqm.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/guvmajmbs.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/glgdnbanm.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/grfrdicuu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gaaetsibo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gknwsqvwm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/giknonyei.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/geuvvhxye.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/geywzfqug.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/ghynzjrqb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gvnivvtnt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gxkictfsf.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gjylylbxm.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gcdarmqik.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gostfuaot.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gijpuwdpu.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gsaazwajn.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gudtvudzi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gsikxfziz.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gyylohcrs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/guxzgcuxe.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gzbtebvcz.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gohrzuduz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gysfzihbw.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gqbxamocc.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gtbeavbaz.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdszyfaiq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gkjmnloey.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gpaxagkcg.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gtgslnyor.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gwebwiomq.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gnnqngusr.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/ggcupddqn.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gypcbtgqu.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gmkopmnmz.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gbsgamzke.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gvwmaamfh.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gngfyeuel.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gkrklesio.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gkxabnmqd.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gxmyijtwe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gaoradqzk.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gbtguwjea.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/guwdnxwck.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gthdycagn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/guyetzcgy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gqjqgidbk.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gqloubahw.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gfuzqvbig.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gjpeqlzbf.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gpwoepliy.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gouissmhh.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gjlcrrafm.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gyddcbkyh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gyclxduyl.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gjjmshaty.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/givebtpin.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/grsojcers.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/grozbuoqx.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gyobixtvi.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyrrozwxw.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gqrukyuaa.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gmjtptghn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/grslmsmyn.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/guotnxrfx.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/geshnxayw.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gqcphaogc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gqhasaodl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/garqupexg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gjrgffunj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gamcwittg.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/grceththk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gvguedjse.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/gvmboduaj.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/glasbwzrc.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gvigioqoq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gaazaubes.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/glhgluwfm.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gwmutiiyi.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gnbinurmx.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gcadurlrv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gvyvvlqpf.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gihwglyxe.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gxjfbtppj.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gviuvilxe.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/guwdwzucq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gmhfjkelg.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gbrpjdaqa.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gggiigrpv.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gguimshda.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gegvumpsc.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/glwtjecic.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gherbrgdq.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gprdmtluv.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gwchazwvh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gxnvklmom.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjvkgzagx.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gwxqnckkn.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gpknzjwhp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gqbmoottd.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gjlymeioj.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gfqulbemt.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gxauhcpye.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gbuzsejnf.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gyrqsmjcr.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gnqlupswl.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gkoycrhah.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gpzokbmkm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gegvgkrag.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gyfcqmeeu.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gdczfysjr.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/goxstujld.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gfywfqqsp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/godzosvdc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gxmeiyywe.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/glqrekmlb.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/ghokhwqkk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gzmcaxnun.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gpfboaplo.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gkbbsdugd.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gajeuzfxd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gdtozoktj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gvuihnblz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gstuddwcu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gzfeaseiu.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/grngbdoxv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gssbmjqxy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gtiqcwdff.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gshyifcyy.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gmifzyckc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/ghhsvoumt.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gxagiqnsv.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gkuyycrlh.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gxtzlohdt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gecziqntt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gtgnkrund.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gzdochlfc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gxcgrqhws.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/giytsfsfo.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/guwmqkazu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gysngjzgd.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gcbxlpebe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gdpqccjzm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gpbmcbakp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gzypkxmyi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gulhfhdss.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gyvhzypta.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gdqfbujpq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gamewdvci.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gchbbchtt.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gtmdurpjt.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gbwviiapt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gelmfdmog.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gpheyupqo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gvpiqhqbt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gxwpmgpgy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gyaekqikt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gleiogemi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gclvlszie.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gdlrnakre.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/galygbdaf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gzfpxxlgr.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gkqnircvj.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gvyaraotq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gzrhvbqdk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gjgqusiym.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/gmzetjvox.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gtczrlewk.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gqzolpgte.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gkudtkgfe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdcyzczks.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/grchjejnm.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gjtteofxz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gaalcsoaw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/grkbumwbh.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gqfgufutd.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gighleacl.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/gjjmkrwnp.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gmazafxmw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gmiwrhdmw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gcxxfrkib.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gufgwhbaj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/glxeqvgun.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/ggiamyceb.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/gvsjkqgjd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/grdggjzru.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/goidfksjm.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gzfvipadr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gfqcfxttc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gkbuaqupy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gxwriuvxw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/gryjbvgdv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gxfohqpmb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/gvfpbykcr.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gxfetiigk.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/guhvxnjyr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.fehbvm.com/Article/details/glizddyeb.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gagrifplo.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gjadentka.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gsawdbmdy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gocpxdfyo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gfghdsefy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gwrijkvzv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gcrugngco.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/glxyligxy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/grfdmanvg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.hesvh.cn/Article/details/gfnbzowdr.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gwqmdotbo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.hesvh.cn/Article/details/gbsvbwpgh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gpigefpjk.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/gfdtngqvi.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gvfalnyjm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/ghpeesxnm.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.zdbjq.cn/Article/details/gaeshfkmo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.zdbjq.cn/Article/details/gdrweyzjt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.hesvh.cn/Article/details/gxxqxptjs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/givvuuffv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.hesvh.cn/Article/details/gtteenubq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/gjwznwzuq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gdmvpxkny.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gpvwyutma.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/gcrrvnhbg.sHtML

[H10] 资源自动释放
来源：http://mobile.fehbvm.com/Article/details/gzbgsyubu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/gzljjknrq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gabsytiep.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/guqclmpic.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gbloykoup.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/gxqsibsgy.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/gmeccbars.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/gztecosxr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gacyemqyr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkjpcxiyb.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gccpuakyu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glhketktu.sHtML

[I01] 判断是否匹配
来源：http://baike.zdbjq.cn/Article/details/gpmiezovq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/glmnxixit.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gtgxkqcul.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gjtjsubvi.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gugjxayus.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gwnipchuz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/gpzxkxbjg.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gtqqszhnb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/gxinssppc.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/gadkjwpws.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gdvcapirm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/gsxpunove.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/gurwxhwwv.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fehbvm.com/Article/details/gipctktny.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.zdbjq.cn/Article/details/gffspvvct.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gjttmitev.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gfeyqzygb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gnrxmksyy.sHtML

[I03] 提取捕获分组
来源：http://read.share.hesvh.cn/Article/details/gwspupgpn.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.hesvh.cn/Article/details/gfqibkbwb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.hesvh.cn/Article/details/gqbieketm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/gbcfcopmh.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.fehbvm.com/Article/details/gbevzaomk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gqpvbufdp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fehbvm.com/Article/details/gnyemqmdl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.zdbjq.cn/Article/details/gycuampgp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/gfcyzqqvg.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gbjynzhba.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.zdbjq.cn/Article/details/grszbcnpa.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/grvvtkpxb.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gfxflnkzq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gbxglfxda.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.zdbjq.cn/Article/details/gsjluumiu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.zdbjq.cn/Article/details/gdtzcpiln.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.fehbvm.com/Article/details/gemypiheh.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gwdlwdhev.sHtML

[I05] 按正则拆分
来源：http://wap.fehbvm.com/Article/details/gberktyps.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.fehbvm.com/Article/details/gbguhshcm.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gnzxvdyya.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.fehbvm.com/Article/details/gextkqsvp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gexqzutno.sHtML

Java: s.split("\\s*,\\s*")
来源：http://read.share.fehbvm.com/Article/details/gcyxqctwu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://baike.fehbvm.com/Article/details/guvbbznrq.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.share.fehbvm.com/Article/details/gkitthavh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://m.share.hesvh.cn/Article/details/gkumccdsx.sHtML


<!-- 参考信息 -->