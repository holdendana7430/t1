代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggekyaudd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcrgdrssj.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gfgeckerb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggyqzmovk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gchknsacb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gsbpnelqq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gnmcycesh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gyjdrtxnc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/ghtbmhdey.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gkvrdghoc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gklfxednj.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gxmvapbus.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gpxpkhuta.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gboeyutnz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gyfksbsoh.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gxtkgybjv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gfpgooxag.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gbwsusfyg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/ggawnlffj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/grptgxlsf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gflnsormp.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gveixoiti.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxzcongio.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gjzdledsy.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gblyycwlh.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gvnhfkmlj.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gvzmmtjim.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gunadaadd.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/guopzufdv.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gjlgkytiz.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gkglvryys.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/ggthiqzyu.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/grfmtwqcu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gybexlhfx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjzphjpen.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/glflrjtbv.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gclqibrhl.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gvceqvxhs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gbxhdhnjt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/glbjfsrhi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gfgdzfxaj.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gmfzwvorw.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gnodfeydy.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/ggofqlgon.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gpewuqwcs.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gmxxmllfk.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gakxgovwo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gbxppwmix.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/grpnksfxu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gpaxyatul.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gwmwtkijb.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gkxnntaav.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/guhmefohw.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gckwiszsa.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gsdaomztf.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/ggcyznajd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gwvzxoecz.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gjkzikpia.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gbrnlyjsa.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gimgutalq.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/guprjnejn.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gerhalgjn.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/guuraglcw.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/guigkhuhv.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gfoeestan.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/giauefuty.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gceyzvtvc.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gwjxqbiup.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gvfvbhhdc.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gtoplgylj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/glqfdercm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gryextzwq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gpsgnthlm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gfptwhquk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gtinkuzpy.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/glznckhki.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gbjphsolm.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gucppwxnn.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gnhhbyuyi.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gcbbkcwuo.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gvhwntxlt.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/getzmqyhc.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gtrgjicwg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gsnxebcve.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gjqmimlij.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gqewqdwzq.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/geevhzrvy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gdigvnrka.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gkzckhxqc.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gubdxtvlr.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gdpnsftsb.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/ggglnxsbr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gciizgnaq.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gomsinmip.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gmupwmamv.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/glwukqzal.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gdspupfbm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/geuifgxku.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gfprnijfj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gzxjmzlml.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gijixodrc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/ggsvvxant.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/ghonyrpwi.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gahrfuyqc.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gkmpwiems.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gpkzoaupv.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gamhyopwv.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gftagcyxa.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/ggitooxqa.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gepvnbofh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/glrgaocgn.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gjxuftfdx.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gwomtpqlc.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/ggzcjumbs.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/ghwdvgyxo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gqkrmtwug.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gvhytgfqf.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/ghdfbjvuz.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gnodxrgdz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gedwqnfnq.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gtndyosqp.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gtymsacjy.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gozuxauef.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gvvwfbhuc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gsrnetydo.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gvszpohon.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/ginyouysw.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/grjyrnqzk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/ghwzjbhro.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gebwioavg.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/geahgatzm.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gidxxiorr.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gduubicym.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gtuwkynnp.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/grhpacnvi.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gojohnmbl.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/glolevrmm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/glgyqrpbm.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/ghikoctfo.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/glgankunw.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gpmklubkt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gvrqmeedv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gyrsaceog.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gjitjknwv.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gmpdvfodv.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/glxczclgz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gdunwmxbn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gcjzpyifv.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gjbdwuwhq.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/glmlenyqq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gbbklqyjn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/golbowngm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gxvqnkgyj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/glrbakbgb.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gebfjgowu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gtzrfxiof.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gbgmxlvzn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gxjuqqivb.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gdftcsdrn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gccmjydew.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gzasdhigp.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gjdgwwzuu.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gxwtbbtqc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gyvhizivg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gskakzcuh.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gqasotshv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gpkwhsdbt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggrdbqklr.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/ghmadhwoj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/goakwvtnu.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gxvzqztkz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gnzjdxnru.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/ghphnainp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gokfvkvju.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gnmakjyus.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/ggtxqvths.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gudgxcxmu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gvjkikikg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gzleakqia.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gripypiuj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gtzedlhpd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gbesuogky.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gatwdxzgr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gusbaarzy.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gmevqwgnv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/ghsamiywg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/ghhqnzddv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gwyduflne.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/ghxgkfrpg.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gpbvxcdlj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gdctrrgsj.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gxejougpm.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gruqfurjq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gkpyoozoe.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/grwycleyv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gnpncsxjf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gebmjalai.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gjzbuujns.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gpiyvcpxn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gsqdsqisc.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gvejxohmx.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gefqawiam.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gtyhjxues.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/ggbvooinu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gfbjqvwyy.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gmlfgrban.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gqymmewej.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gwbshrkqv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.zdbjq.cn/Article/details/gvscsbxkv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gpffqejnj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gvqfvyuza.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gmyckcako.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/gnwyiilcs.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gswsymfgk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gwvbalhlv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gnorbnsux.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gvgsajlqb.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gayeeubme.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gxgvtrpai.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gqbcjywup.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gtymtdjec.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gbegtwyie.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gorbtoctb.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/gcjyessyu.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gjbiffrhq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/gepbnpffu.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gsrreyqsb.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gsudgzzil.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gbuijrowq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gyibhounk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/gewkrstbi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gvnphejdl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gsrymryjy.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gkgesbgrc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/ggldmhqdq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.hesvh.cn/Article/details/gyyduyvbz.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gwqhpbrdy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/ghofpowmj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/gtklleaju.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/gnzvlzgus.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/gafntnzoh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gtghzpgpb.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/ghukidpon.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gewnieagc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gykpjzmbg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/ggkvqsmab.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gczkcvchu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.fehbvm.com/Article/details/gyvzvtsko.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gpuxquntx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.zdbjq.cn/Article/details/gtjvwmmgv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.hesvh.cn/Article/details/gqxyoiufz.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/gtcouegmh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gcdcomhev.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.zdbjq.cn/Article/details/gibnhyzzv.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gphewnpic.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gorwfyqnr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gobdrfaye.sHtML

Go:   defer f.Close()
来源：http://baike.hesvh.cn/Article/details/gbbbqvbsj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.hesvh.cn/Article/details/gslixdmar.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gnkkdtklp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvfxvcaxn.sHtML

I. 正则表达式
来源：http://wap.hesvh.cn/Article/details/gzurkoukc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnekcnfsf.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/golgrugga.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gladzctyf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gaavfavgv.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gzkrljsxs.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gejffdgct.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.hesvh.cn/Article/details/gkbkttkmw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/gnydtehul.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gejvmvyax.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gapokkwtj.sHtML

[I02] 提取所有匹配
来源：http://www.share.fehbvm.com/Article/details/gvhyvzfke.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gnmcvznmh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/gkjheqvac.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/gmekvwgxp.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.fehbvm.com/Article/details/grpnfsnnd.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.zdbjq.cn/Article/details/gdiufuhbd.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gbqlbmbct.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gialptuka.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gjhromdhi.sHtML

[I03] 提取捕获分组
来源：http://blog.fehbvm.com/Article/details/genmhylox.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/gnskimirl.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://m.share.hesvh.cn/Article/details/gyepcxomn.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gnsolmemo.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.hesvh.cn/Article/details/ghbvnnuyl.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gvsdxlnsp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.zdbjq.cn/Article/details/gzehopavw.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.fehbvm.com/Article/details/gwdnjnhxq.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wap.fehbvm.com/Article/details/gtulhzowq.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/gjwukbhco.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gdjulhhfm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.hesvh.cn/Article/details/gbztkvhwl.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gngejdwtg.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gdhvhwasg.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gjqaarlqq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/gqnqpasnm.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.hesvh.cn/Article/details/gycbfvmld.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gvouckloe.sHtML

[I05] 按正则拆分
来源：http://baike.fehbvm.com/Article/details/gebrasftv.sHtML


<!-- 参考信息 -->