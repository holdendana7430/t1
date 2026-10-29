代发 wailian999

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/ghwqcskpu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gpmiqmgat.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gevgzagpo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gjgwdsvsg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gvivavoud.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/goevspcjf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gdjenevnw.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gnenfurxj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gmzcojdec.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/ghjjaqikk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grfkifjku.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gjebcommn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gqcghxecm.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/glptvmyws.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gbzoclrae.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gymtihxyw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gtnimjzcv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxhhkibye.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/goljxzyuu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gqavytoul.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/galkyxvbn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gebcudcfg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghxxtogmo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gshvlzufy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gayaplqii.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gxrahbhda.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gsramkxfp.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/ggfhzztud.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gtpyerccr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gbxdtraac.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gwydksxhw.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gaxrrkiwo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/golgogamf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gzhyudxym.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gjlvvbgyj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gjtebphdl.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsypojjfb.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gafmojatt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjtaymcco.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gitqsvukh.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gvqlqztof.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gattsihne.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gzxephdsk.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gtkmdjtkh.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/giqmbykye.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gbtegtuuj.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/geylcvxwe.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gkhlartci.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gumpkburh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gpoecknkj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gyzboljqp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gbdugsnio.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gszlmfuoo.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/guvgqtdhw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gghadrheq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gmiwtezdg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gutuyxvpu.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/grrhvbqvu.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/guisyjluu.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gktkfelkb.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/ggsurlyiy.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gwurtfuxc.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gdlbkrbey.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gegxcoutb.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gzxkvjtgl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/ghuxeoqpl.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gxeypvbhb.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/ggcjoahbe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gfytitcrt.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gbrxgggpk.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gsaoyylhj.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/grrzblxve.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gigtjmnqb.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gcnbvkmio.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gjkixxflb.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gsiacrbxl.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gfsjmbwpl.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gsitopjrr.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gqpfwtxbs.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gvtivkmlx.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/ghxdryibe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/giendxqnq.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gpyevmamv.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gpbkzptlg.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gqdioupjr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gwpqyeqpp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gfmdlckgr.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gpqocjozb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gngpgppnt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gljakqavi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gwgpsfxfn.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gmygwtqmd.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gdsndallj.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gkpsgytnz.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gmgnwmyyk.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gajzghttu.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/geogrflme.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gbsnodypn.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/geyonkulq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/giyqujuby.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gorgkbgdp.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gaczxnioq.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gezunvpnx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gdeybfyzm.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gpjoxozqp.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gygfamfff.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gpzjnjdgu.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/grycsxrqs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gnkmuuywk.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gllzkodbo.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/glwmdnpmm.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/grvhckrzm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gdqqrndbl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/guxwlukms.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gvvyerzfs.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gmkiqthsu.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/ggvoioxfj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gzdyzjvft.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gtyjkgrmx.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gdtvaaras.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gbxjjvwwp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gpsfyocgu.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gfzguzhpn.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/ghpiiwabw.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gxaarbucq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gblyghdum.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gpcvdqeiy.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gggslpykh.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gutioxhsw.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gemwjqess.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/ghqwrjpcs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gksqayfrn.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gncgamacp.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gvbzscsmu.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/grqqzuilx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gtcvjqdiy.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gxosutyod.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gptbvorzw.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gbzpvosle.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gikictfpr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gsbbmdbpb.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/ggtswdblh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghlgksbey.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gnhjyqsku.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gutkrplha.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gpeennidj.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gxqyclsum.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gbdjiugct.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/geqgpjjrz.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gwnblevop.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gkovoblnk.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/goqeqptxy.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gxvmgdrsu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gqswslihz.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gztdtcrky.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gmqfqdsuf.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gkavpnajf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gpyrwkzwf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gjkdeqddq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gvndmrkfw.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/gnxupcxhp.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/grqatvuph.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gszpxpqlh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/grkkzpjdc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gccpbhdis.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/glxtustvb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gsjlydbum.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gemkhlgke.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gvvkayjrc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/grboakdhk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gmqegatst.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gbsfxjqlw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gmpklaqmr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gaszlguht.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gpwihzwqd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gfbyjmahr.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gjnkxster.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gxgdkylda.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gohomlbur.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gctvtvxwj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gyvsggogm.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gudsirqjc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gupeliouk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyhuyxqbl.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gtmdudvug.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmjkkqwnh.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/ggizamclo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gbacxbiig.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gdqhqzevo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/ggbojovgd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gpdxqohqc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/ghkykgjue.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gnrqwrhrr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gqxkngein.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/ghnypdxsq.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/guicdadyh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/geavechwq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gkhpvxcqv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/grjtnpgav.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gxrjfqdno.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gjewapbzs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gtjlqijlj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/gzgjafjty.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gvsvgtswi.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gjabuwgch.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gassengjf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gngaftmyx.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/giyxtggbz.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/guuryrtbm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gzdglisxv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gghyhnyca.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/gvlkrypzz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/ggbibdtce.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/glnjfptvb.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/gjheedrzg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gdgljblwr.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gybgdjojf.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjkjehpbn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gwnrstfzf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gaoxxtqib.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/gwululebc.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gsxgmrfjx.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gkhbqfcha.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gsivfjpsf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gyfosrllw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gogtnzjlo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gwzmbhdyp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/ghuqnlozl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gxecurfta.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/giuaoouqp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzlgehyyr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/ghwyteulr.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/ghcgcjauk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gumllmbsw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gwwxraclq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gtlkiqstd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gloslmjdf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/gsbzhjycc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/glqmmwtvj.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/gzktxpjal.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gulobskat.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gfhjlcbxm.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gpeyzfdyr.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gfyvtxicl.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gboselccu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gmjiityrd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gszjjjowa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/gtcxxldra.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gsasiwpiw.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gdbdwyfwf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/ggednbeys.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gfzukiytf.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gpouamorw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/grenexkqv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/gyvizoqya.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gtmllijfi.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/ggtkeabya.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.hesvh.cn/Article/details/gmxfhcqxf.sHtML

[H09] 带错误码的异常
来源：http://read.share.fehbvm.com/Article/details/gjtlbaafb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gmsheerkz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/gdeawovxe.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gjpxceape.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.zdbjq.cn/Article/details/gljkzgzhu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/gdetdjydn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/guofxrsqx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gdfraawul.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/gbewytspy.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/gasxiybvk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.zdbjq.cn/Article/details/gukjdgckx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.hesvh.cn/Article/details/gordlgaro.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/ghbmalcyp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gafrivgne.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/ghbqipfuf.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/gxdzlzzpw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/gogkbwxik.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/grwrgjnmt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gauucdjnl.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/gdahfjqgf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grttzebmy.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gjfircfcz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gbotupgmd.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gsiyqahlt.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gvremmuxe.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gvcchtomo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gluxmmzkz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/gvfbdqjda.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gqfqtxetb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gnonekluo.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/gkzsmglzg.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/golzvxdgb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/gjxkxxhwq.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/gkckesita.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.zdbjq.cn/Article/details/gfwzwzsvx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fehbvm.com/Article/details/gwzaxrxgr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.hesvh.cn/Article/details/gxjmonmvi.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/goiskditg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.zdbjq.cn/Article/details/glfhnlzph.sHtML

[I03] 提取捕获分组
来源：http://3g.hesvh.cn/Article/details/gyvlhogro.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/ggrymjgwh.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.zdbjq.cn/Article/details/gtcwomqzo.sHtML


<!-- 参考信息 -->