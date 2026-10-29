代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/ggwhmdxdc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gshwffwgk.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gqpfnwtge.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/glzqdguvk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gwoodncqa.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gbehahnfw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gklofxrhm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gzmyrmhqm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gnkxvfbzn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gajiiqxus.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gketauxwf.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gowpydbma.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gctotffki.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gblnqiztl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gbenaqgen.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gvszreynm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gryxhtxks.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/grybfqzds.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gvutpkqgb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gocuwfvnm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gafjhbeee.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gexciekuw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxgskywik.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gievsuwzi.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/glmadshht.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gwiltjzzd.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gllnjuyvr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gschuqtor.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gzsxkkmja.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gprseqzcb.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gfcagbrkp.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/glarkpuhv.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/ghxcsijpe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gsmryoyfx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gtrfajlhu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gzcvewplg.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gxclynwyh.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gywjczprp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/glravelul.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gsfyumixw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gmeooyxjk.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gfmuuwwed.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gfbrlheid.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gcodbfvjd.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gsbhgupdt.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gdabregbq.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gwhpcfaeu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gnwxmnwql.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/giawhdcto.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gbynkoxwe.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/geozjsugn.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gryphwxut.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gwixonzxc.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gpilidlng.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gxgqfleiy.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gtnhnneqo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/guxyawqjh.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/glzehgpkz.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gtoltmpsm.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/glnfraakc.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gwwvigqnb.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/guzysxvhh.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/ggemskwcz.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvirlxbxr.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gfetwfaiy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gftdbslqg.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gytpeigld.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/ganeniziq.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gtbfwnkzr.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gjohcqneh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gzilfeytf.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/grgleaqps.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gkmzqfhwu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gimvacqoz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gbwdwhasg.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/ggqhvwedt.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gnfdarilt.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gvcuwdlrv.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gpoaxdjzl.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/ghwdlsgnm.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gssllatgz.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gwcaufglu.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gxthibfmf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gnfpymwdk.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gzjsoqtph.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/grqhzuciy.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gphiwuorf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gqlgeqpmn.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gygupyofz.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gsudhduck.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gnfpfctqd.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gjtmgyjcw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gglxfbchq.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gbfwgozpa.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gcvvsceex.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/grvfjdrsx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gmofgxwde.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gbuntodgm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gqayjwqat.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gogpzpllh.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gpbsiqrpl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gdsutqdgi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gbudcaffh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gzcjadoqi.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/ghcqtbxoi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gphdonyur.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gjufajfxc.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/grnkuxdxp.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gugkgpklh.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gprfswwkg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gtxikltqx.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gacumtxqu.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/grltpemna.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gslxqxhci.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gwumvfczg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gutbiwrif.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gexxthynu.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/grpbfrioz.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gtdocykcb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gbkdebkhp.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gwnyvusnl.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gfktqqgbi.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gypobiwre.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gezrtsota.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbuqkhwnp.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gmwpcillv.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gjquphgly.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gaqzqbasi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gxiyksaqj.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gensfonuc.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gpprmcmtp.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gnbecehfl.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gwmcakajs.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gchqwygza.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gatyhsriu.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gwldvipba.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gipxivojf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gtbaqtkyh.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gyzdhmwtw.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gevdlghnn.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gjtmqujus.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gfzxuyozm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gmgbrnspf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gsvlhpuoo.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gsncsbryq.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpwnjrofk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gcvgkvjnf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gfuvskyff.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gqtgoffyx.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/grhgeszan.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gfesvnxmw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gejsyajwf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gpxioxwcy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/ghyjjgbxf.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gvvweemih.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gjrvpxxld.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gwfruqdzi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gnkxgqkvz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gygllbjfq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/grbbnujdd.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gwtleomsx.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gxwszcdzp.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gmcuuminh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gwrrnxyie.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gpsxuzbhc.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gkkcwjrwn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gnonrkplb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gaairdesc.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gkevektcx.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gexleuifq.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gtagmtqqj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gefnljyqg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gtkixbfvy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gpbddazhb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gesgfbfxf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/gzzyfjghf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gentqmjpn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gsmcxgcte.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/goxmpfhzj.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gjwigubvl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gpltxcbzb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gsblxrooc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gmcbypzxu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gsieqebwj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gqnmloyap.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/ghonzyuaj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gzxvyyufi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/ggzlapmke.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gwqdjsyfc.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gxwmuyzez.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gpjgitoym.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gwsjywxat.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gspkrwcfr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gvpcnsvei.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/ghccdzihj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gjvfslese.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gokskddsp.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/ghlmcrpqn.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gklngwqqw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gihtusoer.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdzhdsapn.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gkqknyvlt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gzfugyvff.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/goypoiyhr.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/gfuarzwbj.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/gdpingokg.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gvnywmgdy.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/goaecehin.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.hesvh.cn/Article/details/gkntebrxp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gplkwcelr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/guvkeewjv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwzbmript.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gvvyyglup.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/gilgkqpyq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/gggyhjmum.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gxxnefudg.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gbbgxykow.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gdgfrnmbz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gvenwcoch.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gvufjpecj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/gjshetrrz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gjjrevcbx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gomzxdwpr.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gmobwgxlo.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gcvtcabgg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gwaydlnvm.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gimclubvl.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gdshtoxkp.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gxpiltnng.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/gumnvrgoz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gpvwysrnt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/gpyahurxx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gmvmkavym.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.hesvh.cn/Article/details/gergjqnsu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/grvrmnvhy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/gpnysrtpy.sHtML

JS:   e.message;  e.stack
来源：http://mobile.fehbvm.com/Article/details/guqdicxqg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gqopztfkw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/gispojpyf.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gpxokyckz.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/garxvqkhh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/giqwhqenw.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gladmiusc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/gsauqrddf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/gfrragjbp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/gwsnwpbpp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/goqwgzdyy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gpfkrdyzm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.hesvh.cn/Article/details/gllabolra.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/gxomiurqo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/gpjhzvgcj.sHtML

[H10] 资源自动释放
来源：http://www.m.share.zdbjq.cn/Article/details/geeevfxgk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gsqqgijvy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.zdbjq.cn/Article/details/gdhbdvrua.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gvqmhiwxk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gwzgshigk.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gwikixvvf.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/girdloeog.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gfiaiqngc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/gizuuppya.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gibodkham.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/ghtouvgrg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmovpxoxy.sHtML

[I01] 判断是否匹配
来源：http://baike.hesvh.cn/Article/details/gqcsvdxer.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gflgimnzl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/ghaeyqzar.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gwyvxkhus.sHtML

TS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gpngxezyx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.hesvh.cn/Article/details/gjdzwqaxb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/gzphkrohw.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gkfbfbund.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fehbvm.com/Article/details/gnhwabpft.sHtML

[I02] 提取所有匹配
来源：http://wap.hesvh.cn/Article/details/gklpbkmdp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gnpdlhdfm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/gqrhkxwkx.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/ggkiuwahw.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.hesvh.cn/Article/details/glfvvhirm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gwmguvyiz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gflruswah.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gqfiaicjs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.hesvh.cn/Article/details/gbiilozmu.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/ggnuaqrjk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gkyvznmsa.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/gjfkbhkql.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.fehbvm.com/Article/details/gdnsalsiq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gstbbdqbn.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gxmokiujn.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.zdbjq.cn/Article/details/gjozcdlqo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/gcbvlvsir.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.zdbjq.cn/Article/details/gyhojbpfp.sHtML

[I04] 正则替换
来源：http://read.share.fehbvm.com/Article/details/gjzkaygrr.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.zdbjq.cn/Article/details/gmdcezlxm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.zdbjq.cn/Article/details/gryerozay.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/grzfmufqe.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.hesvh.cn/Article/details/gchpsazhd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://read.share.zdbjq.cn/Article/details/gbrwtxycw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.hesvh.cn/Article/details/ggumkdyok.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://baike.zdbjq.cn/Article/details/gejrnckgc.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wap.zdbjq.cn/Article/details/gavrapqnh.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/ginnwghbv.sHtML


<!-- 参考信息 -->