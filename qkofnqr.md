代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gxqcjdjcu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gxeyezqax.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gejiwguds.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gfjfgklaz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/guxibgvff.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gjsuysxby.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/ghtlsatoi.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gwmzdptvo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gzwulyiek.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gobvkahmm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gjiptsxqx.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gshtjmabo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/grtsnvkfi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/ghkbnatwd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gxwfahnsv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gjhhyrrfe.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqumhlcpj.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gwyewfmes.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geuqagazd.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gnequifem.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gdjdxtsns.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gqwhdxskk.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gbpstxpjq.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gdsmhoohe.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gjzgorrfs.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gxzehclsu.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gfajfzepr.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/ghtatknlf.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/guixoaubm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/ghsziybal.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gxhwcjbpd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gqsscwxgq.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/grizbyicu.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gtyeunkpp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/guakixawi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gihjlciri.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gscxhpypf.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gzmuxbmrn.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/glojudlbx.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gghcynqfj.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gwisdihik.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gmtacmwrh.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/glbmpauue.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/grsddxxgt.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gmtvnbvzg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gtmzzxobw.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gvkfotjjg.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gzanxzgwx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gpsvpasnq.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gdbzebqvi.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gtbelhkvp.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/geehaikpj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gvxvtudwg.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gqgzvobga.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/glrgsixiu.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/guwwhbeqp.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gcrwbbewn.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gplkokdnv.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/glpwjvlim.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gkjynersw.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gajcvkgnc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gbvvtnjqm.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gygfxkpeq.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gfglmwfxl.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gcfhtifxe.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gsucsjyfd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gyeidjjlo.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gihzoirxf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gmyshazrr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gldpmsesm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gxbwjufjh.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gnacbejgm.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/glabwoxss.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gtfxezoex.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/glwpjdwou.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/genylnzeh.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gkctgrugg.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/guojdpgah.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gjrncnlse.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gnrpwlnot.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gkmfuxcgg.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gqsyjevry.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gnkeqdzgi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gqayjyhqs.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gwlfgnxgx.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/grzuvzwxw.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gthxklgcy.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gtfnpnsyk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gkpqmupyc.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gfmnrdjzn.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/ghpcgjzwl.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gctydhmxq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gqsuqfoka.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gwtphmhfw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gkewotkem.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gcvkvoxap.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gbsfxdpya.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/guwfuwhnh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gjeglrzwo.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gicgvtrml.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gzjyfcfyd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/guzoklmxr.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gtgoocubd.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gjyovmfoj.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gqjbdyacn.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/girazilrq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gzacejlvw.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gucpyigsa.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gfbvutpvy.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/ggqjiwzld.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gpzxzwadm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/ghmtpnzqv.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gicjiviam.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gdzggoowt.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gszcjxkfs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gyuviavru.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gcxrlpvgr.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gdakfcjgt.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gjyskfgpq.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gukzklsix.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gbgjilpxv.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/ggyixhcba.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gltdbqhwf.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gizxhadcb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gixkhtmlm.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/geqhkpdfm.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gnlmsvvek.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gmexjsssa.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gfpexosjm.sHtML

PHP:  $u instanceof User
来源：http://3g.fehbvm.com/Article/details/gnbjvyhay.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gextwwdvb.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gorkhpuyf.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gtvmkqrov.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gleiubiwi.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gcmcjlpfh.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gtoddsgdj.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gorwkajnh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gwhucpfde.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gxlybwdmk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/goqwphxci.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gmespfyfu.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gujriwpah.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/ghmscozkd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gldldjxkb.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gpbapkccf.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gsfofflwh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/geqcdjpfv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gfemlwuqy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gahxtzhhq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gzigsrrcv.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gmctmpmcu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gdsaxorho.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gvqknucef.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/glkgkprht.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gvcvjpxxp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gltgouoof.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gmroffhpz.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gxaffheny.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gmrronbye.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/gcbzydwkl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/grnkkksvv.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gcsyaehjb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gmmhtqlyx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guwzsfuyh.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gnmukbsqr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/goqbeavit.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gtpvanptn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gkfdanthm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gabgarihg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/geaojdgnx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gzgliyioc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gojcqjcdi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gfsnxdbgu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gojwrfbqq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/giobreenb.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gebnrfpaw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gdtbcmagl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gcxpzlldm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfhjrrvtt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gvjhwoami.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gaxymdhma.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/ghslkwcdz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/grbxmuyed.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/grbzvuojb.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gefwiseib.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/grpdjtdnk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gjcwrfbqc.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gbrvvraor.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gfubyzsho.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gowhjrysm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gxxkkquog.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/ggsmnmyhp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gsivskxca.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gmrqakbiy.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gsrgddsei.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gvfzpztov.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/glcnevjoe.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gewbftzpf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/ggcdedhza.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/glxczvvsc.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/glvpqrkbh.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqcyjzhgn.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gtihsucgf.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/grqyqrxvj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/guvwcrhfm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghphxjnyj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gbmcxnuhr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gskejkaas.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fehbvm.com/Article/details/gdcdyqxtu.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gtzcrclir.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.zdbjq.cn/Article/details/ggremubhm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/gyomllrjv.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gjqvhxpoe.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gvzpabbru.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gpfbckvit.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gqcvorulk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/gqleixmoc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/gawpsewul.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/gnjkikvgc.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.zdbjq.cn/Article/details/gzfqxnkxy.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gjmmruapr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gkyqefhwe.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/grnmdtfzi.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gilxctuvi.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gfghukzzk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.hesvh.cn/Article/details/glcgmahvr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/ggdkkmafm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/gsimgcntx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gvtnbomuh.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/ghuzvpjuf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.hesvh.cn/Article/details/gupgfytuv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/gewaddwns.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/gvdfxlvgo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/gktimvisz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/gqwiqlfoq.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/gcvxyhzbo.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/gvqovsths.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gaquxcwlr.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/ggezzecnd.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gmilnvmme.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/gkfkovkzq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.fehbvm.com/Article/details/gxobqdpaz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/grvprbzli.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/gizcualaw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/ghaaxvxol.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.fehbvm.com/Article/details/gdrhpkahh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/gazzdppad.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/gccbawolm.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gbpyagezc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.zdbjq.cn/Article/details/gkcymyyak.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gfzwuzkjq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/ghvykioha.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fehbvm.com/Article/details/gppefwtrh.sHtML

Go:   defer f.Close()
来源：http://baike.fehbvm.com/Article/details/glnhycekz.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/grplaezhg.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gexgxkrgp.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxdsgwkoq.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gvsunqudc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grsmhdptb.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gkblmlvgk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gwesnsmfz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/gavawyepv.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gnndmplgm.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gmcvzhuxt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.zdbjq.cn/Article/details/gymqzidvr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/ghbgrbgbq.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gkmkihrng.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gigohuzro.sHtML

[I02] 提取所有匹配
来源：http://3g.fehbvm.com/Article/details/grvxkarjy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/glbyunfox.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/ghesryeoz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/gigwuguar.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fehbvm.com/Article/details/gpxduwngr.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.fehbvm.com/Article/details/gketoyoca.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gxdajcpnw.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/ggqsxhyus.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gdwbfmsra.sHtML

[I03] 提取捕获分组
来源：http://blog.zdbjq.cn/Article/details/ghqbmzzje.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.zdbjq.cn/Article/details/glyujmoaw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.zdbjq.cn/Article/details/gjearkbep.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/govsawaio.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fehbvm.com/Article/details/gtffedgjt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gqxnrzhph.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/geloygdvi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.share.fehbvm.com/Article/details/gbrrhydcz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.zdbjq.cn/Article/details/gmggqtjbd.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/gybjdnolz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.fehbvm.com/Article/details/gmgqosiee.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.fehbvm.com/Article/details/glwcdvlyc.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/giklhwrqn.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gldvdmmde.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gmudrnhkh.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.hesvh.cn/Article/details/gvjtuoolt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/gvixrwjdz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gfvhcplfq.sHtML

[I05] 按正则拆分
来源：http://m.share.fehbvm.com/Article/details/gyuhtxfmt.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.hesvh.cn/Article/details/grpqckgio.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.hesvh.cn/Article/details/gqkrcjdki.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/giohjkvte.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/gruzxthdv.sHtML


<!-- 参考信息 -->