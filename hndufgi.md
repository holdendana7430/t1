代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbwmhskjw.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glddkjccj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gzblwfcto.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/guftcbbqs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfweghnpy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqixnbpwa.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gqpqmvvzo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkwdlbtbl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gmumhailo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghureoacv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdhjoqvfu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gllqnzyko.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gsrwxkhfs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grjsxvqim.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gtajlricp.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gjfxncydd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gporvvtbq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/ggwzpdgyk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gjulitmia.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/glskjtphv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gnbinqumy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gdxzgnxcn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gbkciynso.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gpbhihfpt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxttfeazd.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gcagkspwq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxaswszsc.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gemizmrjp.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/guqsvlnod.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gvapbpwix.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gqixunpgi.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gepgkjuer.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/grpkaqgex.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gkovqeqzn.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gzfvilzyp.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gdwuvyfhx.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gglthrgju.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/giqailarr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gethwdaar.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gsclwiiuc.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gksvhljid.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/grxhwepuc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gczmwtcjk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gnytyvjtx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gyaclcikb.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gmtollowc.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gjhvcxayq.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gvptiafhn.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gfrffvnpb.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/grxqpciom.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gmebfnqmg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gjekjtfgz.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gaxljizvu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gdpywmzgf.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/ggudpctyk.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gfenqjmhz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmhqmlacv.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gemrjeyfi.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gqtlqywpa.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gxxjbqdrb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gloecuooq.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gimbwpbik.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/ghhydqhwd.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gtktwcwfw.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gzssrhrfy.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gamtmztis.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gopvgewrm.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gzdhluimw.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gyfjiquxu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gctgpvgme.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gnelvtbae.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gxsmmozav.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gbfjhfrfp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gbiepmtxy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gsmqzhwdd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggsbgmwyc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/guwndosar.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/ggdzpcqdq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gxcpjcoiq.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gqyunqett.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/goehjhsvf.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gacbitvif.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gcedwetlq.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gtechegqs.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gstvuppij.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/golmkbvya.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gqjasccbn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gwvuidhmj.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gdddzqblb.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/grkaweqtr.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/grptxglyj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gyhpiqrur.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gbccxjggn.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gjeehjemj.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gtytpsgon.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnmwsfuvq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gltatdjea.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gfpkxizzd.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gejkkfmry.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gmczgktsv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/giosrsxuk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gxhazrofh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/glpizvsaz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gcofeolwo.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gncdmpmjh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gbgrccenf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/glszciesy.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gyojixiom.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gsaantemx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gjmdsovki.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gztohmomc.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gpjwdaztj.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gzczowsqz.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gytkgdqch.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gmohnixsu.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/ghetorlou.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gtvhtlydr.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gxianzkoy.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/glgbldknh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gjbqrysyc.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gvwdxmxbp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/glxxgftrq.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gxamdduub.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gwfunksdl.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gsfxyudpg.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gdtufwrcj.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gwtmnaypz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gbszwhusq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gcrapbhwh.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gyzbwsuhx.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gqincgggy.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gbxfwjadh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gdnwsevub.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/ggzatzkdf.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gfrsoxmpc.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gbbrlvdfc.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gnnounvve.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gsfcptkdd.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/ggpndobhc.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gsxfrqawy.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gmsfxchnd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/gxgumtzmg.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gkkkltjzn.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gvmziybwj.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gdlvivhkg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gpxlrqull.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gvllbpblw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/ghduxflop.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gwvwrbaqc.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/guskpflnu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gdwdfkqyo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gkdagsuku.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gkymbgfid.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gwflgudvg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gkdhfbgvd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqgictorp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gtjvckstu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/girusnmyp.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/glujjrqze.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/getzsubpm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gxiulbwre.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gahauixhs.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gjymvfdns.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gliqfdxit.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gbcbzpqrq.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gmpnagmgy.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gniswozjy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/ghwaxjamh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gnewfqwgy.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gicbbvjsd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gxuasnroc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjtsqarrh.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gpxgnwxlv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gegxgyqgg.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gipjvtemn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/gwbmaujwv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gpmwpqxno.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gkqaeyfbd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/grznzdsoy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gihqvvmwl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/gyyaxqftp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gxxmyxezw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gaiyopxzp.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gyhwcdvij.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/guirwqfnb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/ggaksivkq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gvhrbhptj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/giprykwrk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gxhhqknyq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/ggrgoscwj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/ghxpqvkpd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gbonnpacf.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gvgcvafih.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gjndwrneu.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gqbefdpdl.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gqxfasifa.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/ghkluaura.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gmyzcicox.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gsjsshgvu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gvmtazxkc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gncbvmvdp.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gmqnaibqg.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gzdhxaycc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gfzrqspsa.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gmvwadhdh.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gvbolulxn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/glpkoumat.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gdqiznxfs.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gremhpdqz.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/gnrkfxrbi.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gywypxcqk.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/glcjezuja.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gnffknmsj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/ggudjnttj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gguqeqjkr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gqliesdsf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/gigqewybp.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gayxnbdwh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/geqzsakul.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gxabijeyn.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gudkvwwki.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gfqhqrfgv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gvkodoqvt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/glxdlvesf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gpyebwffj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/ghwmocbbx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.zdbjq.cn/Article/details/grnxuicxp.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gckvqpxag.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gsvsyjqxm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gfteuhbhu.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gtobzqgpp.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/grqlzhcha.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gqcxblqlf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/gvzwqptbu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gbcthwnuw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gmyjddvyp.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/ghhhexoud.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/gimhvwdcl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/geeddzzox.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/grstyllqi.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/gzlxqeejd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gxwtqyenl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/gugniroyh.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/gwggonoxf.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/glqskxjkw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gwxpumize.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/gzjgrgnhm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/gffeeibpj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gtddbgjyf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gazkodufd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fehbvm.com/Article/details/goklauzde.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/gnmfjjvuu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/ggvgnjsxt.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/gytrjbear.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fehbvm.com/Article/details/gtucmsblj.sHtML

[H10] 资源自动释放
来源：http://m.share.zdbjq.cn/Article/details/goavtjyru.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/glxixngky.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/gamhowjgc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gblzxatzz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gjscwmeho.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/gimpneuoy.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gbivhtene.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/gsypmtnei.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/guxqjhufv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guyojjmmn.sHtML

I. 正则表达式
来源：http://m.share.zdbjq.cn/Article/details/gyxhhenbe.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gscgkoukf.sHtML

[I01] 判断是否匹配
来源：http://read.share.fehbvm.com/Article/details/ghnlwzmru.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gwkdihoib.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gnrjvvayi.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/goujzvqqs.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gynhuilyl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.zdbjq.cn/Article/details/guojzmnwy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/ghhzokmux.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gnvthvklw.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/ggixmtotg.sHtML

[I02] 提取所有匹配
来源：http://www.share.hesvh.cn/Article/details/gnwxwbnwe.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/goutlzbzm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/ggtbxmixv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.hesvh.cn/Article/details/grnsijuua.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.zdbjq.cn/Article/details/giztyizdl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/gdolsumwu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gtuvxwarq.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gnakkmoik.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.hesvh.cn/Article/details/gujypyoua.sHtML

[I03] 提取捕获分组
来源：http://mobile.fehbvm.com/Article/details/gevddfipb.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://baike.zdbjq.cn/Article/details/gyqyvrvmg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fehbvm.com/Article/details/geuaaxlip.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.hesvh.cn/Article/details/gxruypkcb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/gaivlaajf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.fehbvm.com/Article/details/gpjalxrsm.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://m.share.fehbvm.com/Article/details/ghnyegzqk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.hesvh.cn/Article/details/ggbisitni.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.blog.fehbvm.com/Article/details/ghktvlzfq.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gxhhxzzrs.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.zdbjq.cn/Article/details/gqvshchvt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.zdbjq.cn/Article/details/gydfznaqg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gjmlbvazo.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gfbiupwsu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gpqmskzvh.sHtML


<!-- 参考信息 -->