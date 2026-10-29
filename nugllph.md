代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/goiaotjmr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gfyflpiau.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gitqhvcgm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gijllgoya.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gvrvgvvnb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gifwgvxdp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gzatkembx.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/grqrgyftx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gngwupfpb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/grtlxchmv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gbdadkayw.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gipivbptq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gkbttwpca.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gwvqiomyw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/guxhskpbe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gpkqppoev.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gsdwhmclg.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gxellrspg.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmaxfagdr.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gjlwjerkb.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gbfuaqktb.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gewwrwrlx.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gwgtebrqe.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gwycdnslf.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gwodoirlb.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gbhfmocll.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gbulafnxk.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/grngbxvrf.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gwfgabklz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gdljyoasg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/glytqjjnq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gmkrfwteq.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gmdvyluih.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gulocgero.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gyyzyuwbw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gloppqqfv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gakshkcex.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/glbpenelj.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gywnmctvu.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gctlqrsab.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gskfpsxwd.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/goqqieqez.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/grbltppyj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gsmxgwppl.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gbndaqzqp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gurgcnkvu.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/ghbycvplg.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/glqyllbat.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gicyhvscz.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/ggbysytlq.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfxssaoji.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gtfzzsxfw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gtyruxjvb.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gvvgxewpk.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/ggnxidyqx.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gprszkmts.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gscfbazvk.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gpouwjuhr.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gmumoorgs.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gimmivegj.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/glielrujp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gfkrihtwp.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gaszuybev.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gzdkvxspy.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gqgzcnuty.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gduizkvfi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gbmqcsrdq.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gawozulfj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gqbzylnsz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/grtjzvyxx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/goxmcgoyw.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gjbcpxavb.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/glhaxfqdg.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gfmkfcxwz.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gelucattu.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gljvrsbzl.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gfhkfsmjq.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gyncreedw.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/ghqnafzei.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gippwlpzr.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gzebcixnt.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/glgrdarsh.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gnkwidgbl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gnwslwapc.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gcbnifibr.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gmekdmoyk.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gxvhzcgze.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gmhwcrgso.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gypqqklof.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gzfadlctu.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gfwiuodib.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gzlsghpbk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gscajbwok.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gookklawd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gjturjgds.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/glynjxuur.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwteqjbbh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gxtdbdkgo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gtkmjrokl.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gtktjmtkl.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gehvtqhzh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gayxjvedb.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gdyuynkkk.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gxiznjvaa.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gnogiurgf.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gtergntgq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gsxakposo.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/grspxvxuu.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gmpjjjkwg.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/ghpqsevwz.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/glesbkxni.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gwzjktljf.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gyunfewcw.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gzqhoawuw.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjaegqefo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gdvpicupg.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gpqkairzz.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbhbifino.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gykbyzmbe.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/goaojlkzz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gmxjxlnkp.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtazyncrk.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gpvmbbrng.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gtrdvreqy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gftsuasmf.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gtewzcszv.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gujfpxyfy.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gobsdmuyo.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gdzuqxmoj.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gtrfaojuz.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/grdcahtom.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gtqgcluoz.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gfkfkftzy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gohsmdapw.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/glnuooxnx.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gkbdrlvtk.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/ggnwsmbmf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gzbvjfcfj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gshwglnxj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/grexgyawf.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/ghkfydoaz.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gesebgvko.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gxdmapnxy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gwiemotxk.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gjcpyipzd.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gfzqczvmz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gqlwcfbak.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gmrzstlfy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gfmcizagu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gktdrbudi.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gqibhxfux.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/ggvlmctyw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gwxzhalsi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gfbqmkvhx.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gcednpbjy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/goinwtpht.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gxqkufhsj.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gkzfpkupo.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gfvwwpndr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gxlbekdjv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gduzecugt.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/guzuoxwez.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gishoglna.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcgjuksar.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gowuledzj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghfenunvn.sHtML

[H01] try / catch 基础
来源：http://baike.zdbjq.cn/Article/details/ggidbtjze.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gljsrtfdh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gpgdgziev.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gstnhzquu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gbwprweiv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gfzdknyfr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gnuqscuvc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gxhfbsgbb.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/grfzsqmok.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/goneajoaa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gpfrzcyuk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdrtcljik.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyqlkdwnd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/grwtaubip.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gehkjvaug.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gevnhujzf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gzxyjpusa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gigjaqqio.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gwpbnmalz.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gyrfnkbfb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gvrcfpsdd.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gffjmzybc.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gvxxdotvd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gtkjjcpxk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/gfgrtsxxd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gdxiuftlk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/ghdyexcqq.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/ghmmcfuco.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gzcewoipa.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gyopuxoes.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gxnysppqe.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gnebfsxgu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gfkjdxjjn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gvniigumu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gjgopyvfy.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/gxggoowtp.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gqyjmivfr.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gqexelmuz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gplycdcxu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gqgqzzzcw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gdnibytqr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gcscyvyvt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gcovzfyro.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/godfipcyn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxvovqlcj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gsaedggcg.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/grkokakom.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/grpanqoji.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gihsqjyjo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gxumitjna.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gfecmficg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/gjvrntnsj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fehbvm.com/Article/details/glrptuuxu.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gxrrjsoew.sHtML

[H07] 断言
来源：http://www.m.share.fehbvm.com/Article/details/gguyfhabl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gndmiosps.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/gvidfjaay.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/geawbxoem.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/ggwegtrqw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gglyaekmb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fehbvm.com/Article/details/gdabudpnu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/goiybikxk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gurlhyhjb.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gutdgsfcb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/gndnqkzuo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gdshxkdja.sHtML

JS:   e.message;  e.stack
来源：http://read.share.hesvh.cn/Article/details/gclpltfpr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gcneqnrsd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/gtdxajagr.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gpanmseks.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gwaugjhro.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gbhctkaqa.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gjdpttkbf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/grktehlux.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/gkqevxjxv.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/gktgumyrm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/gzmfwtsnx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/ggslskmbv.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/gmzssbxtz.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/gprpmwjgd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.hesvh.cn/Article/details/gzobslctt.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gsenrlpdn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/gygfhvkxx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.zdbjq.cn/Article/details/gbukfjzot.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gndfxxgbh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gjorstcpv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fehbvm.com/Article/details/getvdnrcj.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gfckvxxwl.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.zdbjq.cn/Article/details/gvivlogtj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gkwspzlgq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtxhreqah.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/gehmraxxg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guykafnoc.sHtML

[I01] 判断是否匹配
来源：http://wap.fehbvm.com/Article/details/gnbuieaaf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gmmvggwfr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gxdrzqzdn.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/ggxyyvhsk.sHtML

TS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/goizhlkoo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/grgpotjwc.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.zdbjq.cn/Article/details/gaoqbsfeo.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gvnjdfgiw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fehbvm.com/Article/details/gnduevnmt.sHtML

[I02] 提取所有匹配
来源：http://read.share.fehbvm.com/Article/details/gdzetrcnz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqfyfrzyr.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/gczazlgyd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/gngptqwoj.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/gxachlwfg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.zdbjq.cn/Article/details/gcbcygpvw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gsiconjoh.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gifrmrqus.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.zdbjq.cn/Article/details/gnbepcciq.sHtML

[I03] 提取捕获分组
来源：http://mobile.fehbvm.com/Article/details/gtnrvaxxo.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.zdbjq.cn/Article/details/gsxartinb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fehbvm.com/Article/details/gybvcebzy.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gkjieuhjp.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.blog.fehbvm.com/Article/details/gfqdmalah.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.hesvh.cn/Article/details/ggzbwnyal.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.share.zdbjq.cn/Article/details/gtemwkqoj.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.hesvh.cn/Article/details/gbdzydgmi.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/gyvugzvoo.sHtML

[I04] 正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gormiyceo.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.hesvh.cn/Article/details/guzmrjjkz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gdzexurta.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gcfyumodi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.hesvh.cn/Article/details/gnnnkvxhb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.fehbvm.com/Article/details/gyghvlcxv.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.share.hesvh.cn/Article/details/gkkhqvuai.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fehbvm.com/Article/details/gpyxzktvk.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.zdbjq.cn/Article/details/gjkpanuso.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/ggbrmbfst.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://3g.hesvh.cn/Article/details/gkcizdazk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/goamzzybq.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://baike.fehbvm.com/Article/details/ggpwodmul.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/giowngcgb.sHtML


<!-- 参考信息 -->