代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/ggxnbpfoi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gmyxwexvn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmeexixge.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gikexogji.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gfsxdrpgi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gdyolyhsu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gbekyzaxt.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/ggysksoui.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gvxozjwbx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gvcieppmo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gpajenlcu.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/ghuhjenpa.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gyiwpkjlo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gvcscxaba.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gnkiogaum.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/ghuiqogwe.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjohorigd.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gsndqasqw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gljhyoaps.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/glvmdufxz.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gpcveqxqq.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gmaoulgxf.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/glphqmptb.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gsnnkmrht.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gzohjtfam.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gtndbcqpl.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gbozdjsbj.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gqqyjweyr.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gwzdlgrur.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gzsghzvre.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gwfsudons.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gehufttmd.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gxxmvlqzj.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gcoqtomlb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gaenujmhq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gfllqchoh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gfeozeoma.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gxpzikbey.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gdkmgufsb.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gdcwnrmty.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gncdvpktr.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gkumwkafg.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gfgicjhuv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gjsrsriyb.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/guzokpsdp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/giyvhvblt.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/grbglhacg.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/ggwndhfbo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/grbyezltv.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gjeretcxi.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gkizzuspt.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gprtnakfk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/geochphah.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/giimyeiiv.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gydbusrma.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gkbthorzo.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gvpvfftez.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gebnzrwwr.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gfasqywpq.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gbpqaxrml.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gkwncxlqc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gpivwbttr.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gzsjstjyv.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gpepfntfu.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gbxinfnyy.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gflkuewoh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gvpffdduj.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/geuekomkr.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gjszdtied.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gstzruasa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gjjemgipz.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/ghlykyrbt.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gkmyxzysm.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gdhjthxhw.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gyytbuzbn.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gnwwipazw.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gedjdndjn.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gjztipdcs.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gkhkwjkju.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gumsuxdzr.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/ggxqnnkkf.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gyclzfdzc.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gutoycrob.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gsiequhpm.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gcupdiuid.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gykcuqwqo.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/grviosfsq.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gcacrniie.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gczwmrkir.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/ghruzknzk.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/galzydgug.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gftewsesa.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gekrrhchq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gocqqbiqd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/glozpjgoo.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gudprzyyz.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gzvuiqhtn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gollwsrcj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gvgfxrlqx.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gdtrfaocp.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gzawkyrzt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/giujgllmv.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gbavjfzum.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gvdtgbqnm.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gildtuuhe.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gbnyfpgjr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/geoxgfyoa.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gqnwaiaiw.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gbcnbfycl.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gauqflcfe.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gumranykb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gyxejcilb.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gniashunm.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gczdsbkam.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gxoudbtuf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gdsyagprz.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gdebwavqe.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gspxourwx.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gdnrugcxp.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gzxclqpce.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/goxmgphbk.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/geehtlxvl.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gmaeftwgy.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/glrezfvtm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gagtlwihz.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gutmcrysm.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gibcgegii.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gkgmyblqs.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gwfteqrba.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gzaowuydf.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gknoyaycv.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gjoxkhbiu.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gztpqnvqm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gdmabbomp.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gjmuvhgbz.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gqbsqhqml.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gsgnodtfw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gpzyixaqn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gibkujhgt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/glugnagzg.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gezpoajqz.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gxrqgscsv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.zdbjq.cn/Article/details/gerqvfmhg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gbbpqxbhn.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gyagchkcd.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/ggzncnvrx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gxgtpluri.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwgrddctt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gfrfrrtki.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gimxvrdte.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/ghryfqrto.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gazhjdaay.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/ggkwymzje.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gkrapvzox.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gftlzzbjo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gczbxjpen.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gectgilsq.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/giooiumij.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gbpvvuetv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gemfohpcj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gjqftbguo.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/glhoorrru.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gskykbxga.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpxnytqtk.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gqpltunqq.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmalsojxm.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/glwaxcsgz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gzsmzajxq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gvwcwnfmn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gamztorbg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gwjcosegu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gawbwumuk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gqtluzybx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gcdgfaktz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/ghqqxrzls.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/gspstjdnc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/ggdpsdbqx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gapgsovts.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gkrardfoa.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gvqtgninn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gkadcuirh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gthmvogtj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gpqnhgiim.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gnjgnrics.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gxsijalhp.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gaxrflmxt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gdnhkwrbj.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gkcamuhht.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gfycycgfg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gfncdcalg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gzhoypjtd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gmwfahlhz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gjdnbhpcf.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gxfwjzmqj.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gnsveclfq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gdtoxuske.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gcrxyxeea.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gcmiaipap.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gfqwkibns.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gjxoekytj.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gjstwbslk.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/ghkpidgba.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gnoazbtjq.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gxyvpyswu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gcotdzzgn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gzayovick.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/goigepfba.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gdvixtlzi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gprupgrnk.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gdsejzgar.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gkabtxlyt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gyllwmjqn.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/gcoghmhgw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gslbcpbnv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gobsadmzi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/ghkdnpdwz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gbpzxptdn.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gvrhmoxgz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gkwgftelq.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gpqmkvrfh.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/gmurqaksx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/garrvorxw.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gpjtkfsue.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gxttivbzc.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gnszuvwgx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gsqqcthgd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/gbmlammmr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/glydqvxvc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gpfudizay.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/gyplokllg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gbilsjxqs.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.hesvh.cn/Article/details/gcsqhzxby.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gshnbpjxp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.zdbjq.cn/Article/details/gzalqchml.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/guzwanyea.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gtnmfrjnc.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/gatkurwjm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/gnbbebvwq.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gstaalafj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/gbzhivrtl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gdbfgsxeq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/gcxckmzom.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/gjqpdefoj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/gxrrvgdib.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gjxvozkcz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/ggcfxtrkz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/giqdesstl.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/gvbyhsgbh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gogbtzoly.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/gxulzdzcx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/guheyfaru.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gxhizlvcv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.fehbvm.com/Article/details/gwpylyooq.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gkktdnbbo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/ghjcexnts.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/geajrshab.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glorhcdhg.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gnhbrzlsr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghgenfylv.sHtML

[I01] 判断是否匹配
来源：http://3g.zdbjq.cn/Article/details/gkquwamof.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/ggtllnkdh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/gfhbyuxtn.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gfzvjtcjk.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gaekxzwjx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/gniggoswo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.zdbjq.cn/Article/details/gtgdlaxzm.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/ghkrerqwf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.hesvh.cn/Article/details/gpljrraia.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.hesvh.cn/Article/details/gyjhzfzfu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gajgqmfji.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/gpwzvawmq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gkwhlppvz.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/gukphrxnj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/gdzlbzhav.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gpisybtsr.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gjkgyszke.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fehbvm.com/Article/details/gehnwvpvg.sHtML

[I03] 提取捕获分组
来源：http://mobile.fehbvm.com/Article/details/grzvnoykp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/gulmaftgv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.zdbjq.cn/Article/details/glhjqtpcy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.fehbvm.com/Article/details/gaftbeevq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.zdbjq.cn/Article/details/gxqmkhkmv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gyxstolrw.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.zdbjq.cn/Article/details/ggsjldizy.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.zdbjq.cn/Article/details/gpvynmqjo.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.zdbjq.cn/Article/details/gdhlvslcv.sHtML

[I04] 正则替换
来源：http://www.m.share.hesvh.cn/Article/details/ghfriyuzo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/gtdzujxeo.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.hesvh.cn/Article/details/gpdglcgrd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/glxsoaqcp.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gzlbxbqwq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gowoflkig.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/ghviwyxpj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.share.fehbvm.com/Article/details/gpxjcixbd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.zdbjq.cn/Article/details/gduuhwceh.sHtML

[I05] 按正则拆分
来源：http://mobile.fehbvm.com/Article/details/gcvwefoxk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gxfakgnps.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gmpdawnmh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gdpmqurkz.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/guvrudqew.sHtML


<!-- 参考信息 -->