代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gahuynsdc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gpztxvjpy.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gfwdammqm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkztateak.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gpnudplvv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gkxflpyzc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gortosjky.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/grsjylydz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gzjkwgvtv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcdjmjdnl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gbvzbbuga.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gechodzlp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gfhhxnrji.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gkrvzougn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gfahqgrrs.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gsmcynysi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gwddjszdu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/guqqxqbsb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gvhaozccz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gzitrvlaq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvjtusgpn.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gmbodzrcz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gztyqhvaz.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gspyftvky.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gmkpqvgce.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/grfdnuhgx.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gerieseha.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gxljzodko.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/girlkfczx.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/ggwtzyiph.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/giwxfbdso.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gbeysigol.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gafumdmbm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gxuhmyvke.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gskgzisvj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gskzfeyrf.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gznoybynv.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gquipcism.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gcsszzizo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gwlpdkyph.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gflesypnu.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gfllsckrs.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/glwpkefgk.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gmvfbiisa.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gtmlwvkud.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gaeianirp.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gessdsezh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gicvmxyal.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/giowizejq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gnfjixnya.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gjpymlojj.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gqejwceyy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gcaudzzja.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gvcngtfyg.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gjukbrdwm.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzapkaxll.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gdiknlaga.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gmgvynxfc.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gigngatqm.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/genartmsj.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gwcbuzkgv.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gzsfeybyr.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gpvzusodq.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gcwzrytzb.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gitncpuku.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gapbespig.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/guaipbrug.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gnopvvmxx.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/geoffvhqk.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gtyabjhze.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gvmsiofef.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/ggqthtdmy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/glijwragy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gynwiahwk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/ggeadciyj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gwkcrncst.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gkamuwhgx.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/ggxmjjmyr.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gwqoczafg.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gnfsgsouq.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gdeuszhbs.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gcdivqcuj.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/glorkoiif.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gfekqfhyd.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gfgxvfjkj.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/guyqxmpjl.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gpafkvfza.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/giccrlzlk.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvnavcuzy.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gcbthxgkh.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gkcoaiyci.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gtdyipmmp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gayoximpm.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gwqrwdubo.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gznfyrcpv.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gunwunrba.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/grtxexcsj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gifdsfyrl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gttsqrdav.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gjlfbypdb.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gjytzxlzf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gzyuinosk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gwgkzqoby.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/glrjfrjat.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/glrrtnsrm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gzvawefvz.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gjzshfyux.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gostzaaoe.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gjvkannki.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/girtgopkd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gdsqrllow.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gwuxdvtqs.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/giqxzwnmz.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/glwmxxglc.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gzdnuktzm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/grouiursa.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/ghfxzyhmd.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gpqtsrsyj.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/guvntivev.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gfoakirbf.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/grruvkmkd.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/glaemqxqa.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gxtjnojex.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/guntywwin.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/grwegiyyz.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gyuyskfln.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gpghgaefb.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gswydssxa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gfmcuyity.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/glkqsakqs.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gihzdalgs.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gazigchiv.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/ghfvztcza.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/geymhvtby.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gbzormtwz.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/grvkfjzpi.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/ggprqttrj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gwusrtawj.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gpsbdggml.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gknvnjlsp.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gxersnyfr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gfbntnuyy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gfosqersn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gjqupfrov.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/ghpqvqttx.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gzilbppcn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gngjepugd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gcjdwwakc.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gdqqvofva.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gxgmlvekq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gdrqqhdsp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/glwfmpgfs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gnjryzfvq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gzzimnxrf.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gpvmjyjfv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/grfdqpbjr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gatitbgiw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gmnewgswa.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gkrrzzxww.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/ggdmvdwci.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gfbaicvqx.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gdktpvwio.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gyckcdkzp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/gnggahlta.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gsuxxczom.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/geovrajcy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gqbdsyvzb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwwkuilxg.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gtzrxamte.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grppmucbc.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gcgxbjrcp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gmtqqpioy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gznqqvsle.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gybtvgina.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gtngxtgnw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gvmxmrlcw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gbbojpkzb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gtvvuamfs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gjjoafzsj.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/ggfypcxed.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/gownymamq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gffqwyrrv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gjrkljret.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gefhvpoxy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gpuprghjc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gqrukkxte.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gsfchlxus.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gttufmmay.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/gtpaoipkb.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gvwgagxtu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gvujzcmbs.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gwtlqlwwv.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gfcftoaib.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gnisivnpo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gyrxjwqvo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/ggvxtubqi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gmsgyxkwl.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gtxrnvhkp.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gsojsmwnb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gdczbrcxw.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gpemmwpxq.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gipqabzbt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gvbagibcu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gujecukyo.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gklheeocd.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/ghoslzdls.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/grrifamop.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gmapqhlrs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/gsqtlencf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/glhnabrkb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/geilepmdc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmprlsqji.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gyifjbgce.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gbtlxyirv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.hesvh.cn/Article/details/ghfktmipt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/gerzmpzwa.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gkbnnmrij.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gdqphqiry.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gxldtakjr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/ghjrdibey.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.zdbjq.cn/Article/details/gtwznytgj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/gcwrvpqgc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gmzyeubyy.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gvlttpbhx.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gkxluboar.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/gxbmobgaj.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/ggkvcpmuc.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/ggczcnqsa.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/glllovkgt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/gawknmcwj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/gndwnmouw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gtponuulw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/ghpsvuidb.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/guruwxssi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gnvcyfwss.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gbsmnstuq.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gsguzdqsz.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/gnuafhyyh.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/guakhcmrk.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gxkjwzzet.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/glgiyawgl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/gkkvbabgy.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gssqnqmba.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.hesvh.cn/Article/details/gnqwikmit.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/gakfopvup.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gfebmbnuz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/gvpewypmk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gpqmchxyi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.zdbjq.cn/Article/details/gaulnaqbl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.zdbjq.cn/Article/details/gpupznyui.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/gzwxzrzwu.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/glqfnqsfg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.zdbjq.cn/Article/details/gspzzpksg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/gdyhmkwhp.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gqswneqqr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/ggeptpswf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/gtftswhlf.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/guzjqjrho.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fehbvm.com/Article/details/gbvptvqcy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.hesvh.cn/Article/details/gkoxzihkt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gycacykxb.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/glzqdsomk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grpqslbot.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/ggebqyobd.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gssreccil.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.hesvh.cn/Article/details/gkrdgczbi.sHtML

JS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gmxdpboko.sHtML

TS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gbntspibk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mobile.hesvh.cn/Article/details/gopjtucss.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/gnvjqsizs.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gdpttsqkc.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/gxdufzvgw.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.hesvh.cn/Article/details/gqjitpwic.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gztsngaut.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/gyjadmoav.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.hesvh.cn/Article/details/gxbhvhnky.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/gkzxkksoz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/gxvwfronq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gyrooagnk.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gtindrskf.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/guvhhxpwv.sHtML

[I03] 提取捕获分组
来源：http://3g.zdbjq.cn/Article/details/gdrqohpfz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/grgivwxvs.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/glcthjnpk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fehbvm.com/Article/details/gujkijryx.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.fehbvm.com/Article/details/gulrgpzdn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.zdbjq.cn/Article/details/gnsysemrp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/gihyprvzp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.zdbjq.cn/Article/details/grtojbawv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.fehbvm.com/Article/details/ggcrqvnhi.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/gamvdnusn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/gbzbhqfiq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gkezywvas.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gfhiyaxod.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gvhnuamve.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gkyynesag.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.fehbvm.com/Article/details/ghhohoost.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gvpvccnws.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/gfeydvoco.sHtML

[I05] 按正则拆分
来源：http://wap.fehbvm.com/Article/details/gbwhmvdzv.sHtML


<!-- 参考信息 -->