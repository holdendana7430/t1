代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gxlcdvgbr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/ghkuqagim.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gzzkyplwf.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/ghbqgsuvs.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gcnqfydlr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gvusaoszx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gaebrwmkv.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gdbbadjki.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gptzgysei.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gmszsfiui.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/ghnwoojis.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gdcsucomi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gryuvmcod.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gmytjfjao.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gatgwnhwt.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gglthgywb.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gpuotlitg.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/ghnmjaexk.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gwsnffsps.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gkseiahjj.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gpvewzqrk.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gwnajnpyy.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gskhizwtr.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/grhzyrumi.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gqnefmobc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gbffwlflo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gthmhyiww.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gvykppsjo.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gpfzpziwb.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gjzaaepos.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/ggylbkhbd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gsnxvhulj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gjryajpme.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gaphqikxb.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gtvtfzphb.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gmhqeopqg.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gmyqbfwqc.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gxzrcacix.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/grjkactne.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/grwxuiiuq.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/grnvaiuwx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gdxkapttg.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gqucdcoie.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gdferbrev.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gcyzltvoq.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gyklpmbpn.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gaddpohmz.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/geyzokoqt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/giwrztzyi.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gtljptvxu.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gcqthmqrp.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gwjcssylj.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gljurtgmu.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gbqtklydr.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gzbmwivhj.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gghgozcxl.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gwbuwlohf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gmlciousi.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gdvfrkiip.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gvdkklymz.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gasiibfoy.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/goqhmpbzn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gnahkrqcw.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gavkhkcsd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gligjjzzu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gxgsyrrup.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/ggihzafxz.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gsstlryby.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gvjztxkig.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gcbbvgjfn.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gygvroywb.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gwstnbmgg.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gptwjblyg.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gkdspiwjv.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/giwqaigbd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/ginghvlds.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gzorhprbd.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gvbnwictt.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gjbchlrdi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gffjivpta.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/ganvzpafz.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gkfafqmii.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/giipmqvlm.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/goyvrrrwq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gaqinzjfq.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gbrrnfkby.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/getsswwet.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gsaoozxzx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gkiangnmj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gppnnjskb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gokpkgluh.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gyyzhfxep.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gwyiwmvsx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gecdsgjzp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/glehqoszr.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gzlbboshe.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gtrgqhkyr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gfguobsmb.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/guneomiqf.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gqwjcloyc.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gtfbpdypb.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gmfudqtpx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/ggstxstmc.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gctpsfstv.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gbmlumgtw.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gcoajsmnj.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/giretzlpe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gltwhykqv.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gcmedshrm.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gmmvpbwaj.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggdkeqaex.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gccqbmymb.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gkpbkyqsh.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gkygzglhj.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gndebfqve.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/glgjmkhyq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gyfprcvwm.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gcomagxjz.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gfzyhyxdp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gxykmmpkx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gbewxfbcg.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gfsxqjzsu.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/garrnbmet.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gquvycugj.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gtoygmhmb.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gxaxutvxi.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gkzylmuon.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/grsogvzww.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gcdorvznb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gdesrmqym.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gippgbijl.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gvikmxqdr.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/ghmsfjbvg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gqflxyvfb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/geuwwptqa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/gkrgpjbwp.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gydrhdxda.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gfunnaykz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gfmmxmrgo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gvikutgnv.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gzuacerfr.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gdfninjrd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/guejfuzqh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghdeexhrq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/ggsytpnxi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/glnryluxy.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gvnpnhswg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gzeaovwho.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gmpnjdjkc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gwthzmdwe.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gjwwpedfx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/gywrztwth.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gjkkccldu.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gmjkdsaut.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gopqmskeq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/gjrqbuttm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gfegymquh.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gtyzvkcoh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/ggenltdzq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grrbolqia.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gkdshshet.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtlsgkkta.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gvzhukcyt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gqhsyuhsw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gpdsjtmad.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gruvlmnsr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gfhcplhgb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gbvjpowuh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gcecqlykk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gtqgtfdax.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gskzmnwqb.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gkfvnitjk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gifhvugoj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gxokfgbjx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gokxozjvu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gjpjhfaip.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gfoqklbtb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gmvgbnuna.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gadbdwhlx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gkjagdbkd.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gefvktzru.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/guvtlqxbg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gjlgebvwq.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gpmtwxlfn.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gapniqjzt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/glozdjxnj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gefcrcrkb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/ggezfnqaj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/guahgaqtw.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/gsgoadqar.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gswsjgrke.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gnvdldlwp.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gdshqvntq.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/ghlecniwf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gcrqlmonc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gtlphyovy.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gkwinhegq.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/ggsuxfxdl.sHtML

[H05] 捕获特定类型
来源：http://baike.zdbjq.cn/Article/details/ghmhzifeh.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/gtrudtytz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gtivuzxaw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gfoxpdkkb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/givtlesgb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gpmciocdn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/ghziunmuo.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.zdbjq.cn/Article/details/ghxbjvspm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/gxzsfgase.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/grrlvefjl.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gpkiketwo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/ghwtctqfz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gwcpnzyrq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gkffamlfc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gnvnakpop.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/glvzeimfi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gnoqpbdwl.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/guxidbvyk.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gpwnbkoek.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gwzblihbs.sHtML

PHP:  assert($x > 0);
来源：http://wap.hesvh.cn/Article/details/grlemkpiq.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gkywcefey.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gjbrktleq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gatoepnmc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/gjaozpdfs.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/glxstnhlf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gunqydmdo.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/gvorzmnvs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/gsdoognch.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/ghxpeohjp.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/gbzakcvoy.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gbgswoukk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gbjifcvlf.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/gdjxsgmin.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gujxqvwxk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gxybvbqfy.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/glomessyp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/ghgiibkpg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gkdkeqtgs.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gjmqegdjr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/ghmfrqmcn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/graofhenn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gddpevxgu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/gctmogvhz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/gytomnbig.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fehbvm.com/Article/details/gplncmkyv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/gwqqarqwx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/geuqgjqpr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/ghgbztfak.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/guinqkwxz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.hesvh.cn/Article/details/gkeulhqsf.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/gdufzohke.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.hesvh.cn/Article/details/gveeluzid.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gnsykcotk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grhngwaxe.sHtML

I. 正则表达式
来源：http://blog.hesvh.cn/Article/details/gliwyaofo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gaavldkva.sHtML

[I01] 判断是否匹配
来源：http://blog.hesvh.cn/Article/details/giahkfdmf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/glhypjbiu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.hesvh.cn/Article/details/gjnwsttrc.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/goimykzly.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/grurfevno.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.zdbjq.cn/Article/details/gjfmrhsde.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/gclvonjuh.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/godfblwws.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/gaisjltxt.sHtML

[I02] 提取所有匹配
来源：http://m.share.hesvh.cn/Article/details/gtkdvkgcg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gchhgyvxm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/gknhusgfx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.fehbvm.com/Article/details/gyorekynp.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.hesvh.cn/Article/details/gzaluaarz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gxpdgnadw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.zdbjq.cn/Article/details/glxamorpa.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gmuzodwrd.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.zdbjq.cn/Article/details/garsnphrd.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/gljtltwja.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/gdhmgybxb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fehbvm.com/Article/details/gjbyabluv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fehbvm.com/Article/details/gyfhesrsp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.hesvh.cn/Article/details/gsbbkizhb.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.fehbvm.com/Article/details/gstnxxamv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/gfxjfofnd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gfymfhnfz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fehbvm.com/Article/details/gurpigonp.sHtML

[I04] 正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gkprjrhda.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/ggwgwnkie.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.hesvh.cn/Article/details/grjjrollu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.zdbjq.cn/Article/details/gsgolzqbc.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.hesvh.cn/Article/details/gjyzbhomx.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gbveyeqeq.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.hesvh.cn/Article/details/gzcslraen.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.hesvh.cn/Article/details/gpzltmgpc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gpiqonduy.sHtML

[I05] 按正则拆分
来源：http://baike.fehbvm.com/Article/details/glbfksijm.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://blog.fehbvm.com/Article/details/gkvkmthks.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://baike.zdbjq.cn/Article/details/gezzsynrp.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.zdbjq.cn/Article/details/gzxyygkcx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gehjykesu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.fehbvm.com/Article/details/gzbctaslx.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gsksxjucw.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.hesvh.cn/Article/details/gozsulcnh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gymwvapnl.sHtML


<!-- 参考信息 -->