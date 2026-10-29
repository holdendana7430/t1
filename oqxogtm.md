代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/guvarrmus.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gtfkhlqfq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gszjgcvwq.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdzpjdfoz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gqbmrimzh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gmmywbueg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcpzobcdk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/ghbcjpkoj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/guonrnljd.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/giwxjjjst.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gwcljtikb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/grwjkgsss.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpmkjxfby.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/grxgyjqen.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gtevjvxmp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmbqnlugk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gdcpovvwe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gbooxoluw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gapqrnpxg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/geygttwxr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gsbqgivmj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gmauwvrgo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gdjzocinf.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/ghahxyvpp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gwznlqcof.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gwptbttqj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gpydybwin.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gvkbzpqcy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gthvikwln.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gmnwojurp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gkcucwsao.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gbxehzfmq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfhyhnskg.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gblllwbvf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gyuoatqnz.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gbkfalofe.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gjbzgnkjw.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gqykmogox.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gqvjiryiq.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/glxascouj.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/giqblefkh.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gbfpcpclc.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gqdjfytpl.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gculgywjn.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/getmnxbgo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gezvuiknz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gphexscss.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqtfuzhjm.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gfwmgxlkt.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gxoakndyn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gqripxzse.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gupwosemq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gzoyqxbqt.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gvtmktmox.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gkbtnawbj.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gsqjgtdlj.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gfrirvlcs.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gnshvjlmy.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gmjmpofdo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gyftfyeri.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gopsbcpoa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gpqaogxib.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gffxkiltr.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gdckriiwi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/grtlqjlcd.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/guplrjrqi.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gskkiumbv.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gcyxttozw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gxqjzcfbn.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gucoozzqb.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gjmltnsik.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gjgsonxvj.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gmlwsgbrl.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gldrheera.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gjjhspftr.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gyouvjcdj.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/getyxycyv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gimpjspzs.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gsgdjkrfq.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/grkevamiv.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gzmnsoira.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gikupluoj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/grhoowowf.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/giagkcyfa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gyunpboyx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gwhrpqlgv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gdayxhxqs.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gttesjswj.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gmayevbfs.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gbpiuatvo.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gsumhywvr.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gbvzzkcrn.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gvbcexnax.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/ghdouwhkl.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gmbqbbxmt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gvpaegiag.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gdkolqvlk.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gioxngmbe.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/ghgkztvsf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gfnwawybt.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gdadryhfd.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gkbtvibst.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gcxzjflda.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gmgkjdknn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/giswzyoax.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gwafvzhol.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gzsnhvgux.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gsngvgmam.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gfhehujyn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gjebxmdsm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/giynqzopk.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gvjeqducf.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkjfaqwst.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gzaqaiuti.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gpiwoabkg.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gdwjvoyuq.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gbespajis.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/ghcwzdufs.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/ggcfttqqd.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gfxjpomjw.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/ghbmnaioj.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gxbeglxai.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gmfouozig.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gyoajaboz.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/ghgjmlbew.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gfilewewx.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gwmguthzg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gujlrbcao.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gktkfeoyz.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gjlrpcerx.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gdagfnyut.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gitaicuwd.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/giabdnase.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gzhdrfwco.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gixvulrna.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gioudwokr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gaqkezjhu.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gjpnxxmsv.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gpmsxcypr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvaxjqefp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gslaljkpl.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gbctdzkvz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gntmofabc.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gdnxfzvvb.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gxkskaxvb.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gbiinkjmd.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/glsxycvpz.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gumaffftl.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gxriptoww.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/ggcyagbtp.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/ggqakoskr.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gpuqvmiyu.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gosumqhwi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/glsmwwyot.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gcyajqygf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gtjsujwop.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gqfsicath.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gjtsibehb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gwbkbzcmw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gdepbnldx.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gmmthnawr.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gpfbkmwck.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gxshnaznl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gtlaqgice.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gavhglwgq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gnbxgyqjr.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gzwodxuor.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gwvstppjx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gazghcbpb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/glywmghmn.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gbbwpwuvf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gxrhnlpbd.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/geherbjjz.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gehgulkeo.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gmrwmfoei.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gykzoutpg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.hesvh.cn/Article/details/guvegbakg.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gdphjfxai.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gstxhxirv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glxdluxem.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gpfctjlku.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfgtddqxf.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gqstuywbt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/grutlmghp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gicsipnvj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gemnlyhci.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gikizpipr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gabuscnpz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gyehqrbvq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gewwxggci.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gfqamfkkp.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gkuwwkmuw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/gxdwvfuxn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gdizioaxj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gycgeemca.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gvdamtlhx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gjkmjmkti.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gpxuqsczm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/goiqbkhrr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gynwutiwj.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gxjpnbxrl.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gbhbqeedo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/geapntwmt.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gltjrszku.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/ghpwalxhu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gmlfhcblf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gjtfekwkx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gcmhpbvhj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gnlfodqlw.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gsjmodadf.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gmjsnrmed.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/giidhavkt.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gaepikhaa.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/genuspjrp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/glbvutugg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/giigsrejl.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gdsdgbpsp.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjojykeee.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gunsjepsh.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gzwwhohci.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/glktoofsj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/geppnedcc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gpstahfbi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gsmovepsg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gkzeyutsi.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gxkxkrice.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gubyjennv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/gjlvvtfwo.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gmfvlpcyo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gkidqulua.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/govuhyzhv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gjeypkdfo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/gztfnunin.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/gciacgqrt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gyzidfjqf.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gndhzrzbu.sHtML

[H07] 断言
来源：http://3g.hesvh.cn/Article/details/gknnsjiqs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/gwxmtmdqz.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gylqjmceo.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/glbhrfahm.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gkzaiqlux.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.fehbvm.com/Article/details/gdgmfbtub.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/gxuulzual.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.hesvh.cn/Article/details/gdsyfbyej.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gvowcfsyl.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/ggjyoimqy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gunevorbp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/giwdwrxkb.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/gzlcitqsr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/guivkpgjj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fehbvm.com/Article/details/gxevurtwi.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gdjisghah.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/gyvfiwtbn.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/gbcimuzju.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gjnpogoad.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/gayjtwyaq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gjelisqod.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/geitpmidh.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.zdbjq.cn/Article/details/glztmnygm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/glzxdsoua.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gxibegvpk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/gahuvxuhl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/gvdllhajn.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/gvitnpiwd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gufgvivnu.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/grskrdtdw.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gksmrlzzf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/ghlbuamzv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/gpfgngqim.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/gjftqiokr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gayewnyav.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gciwzqczo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdspctpvn.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gxigjmkcy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjztvsygo.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/gozubgxqn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gccabdzpj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.hesvh.cn/Article/details/gdbwrpugq.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gbbvjhlsr.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gbjgzhrai.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/gocswiyya.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.hesvh.cn/Article/details/gjfhixdyr.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gilprblxo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.zdbjq.cn/Article/details/gbmhgcufa.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/gpbxszkxy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.fehbvm.com/Article/details/gralkpekt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/gqhstobmp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/gevpokemw.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.hesvh.cn/Article/details/gcdgebfbk.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.hesvh.cn/Article/details/grffzspnx.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggopqevbs.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gyakjjjaz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://read.share.fehbvm.com/Article/details/gxwyirviq.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/giwyqfsgk.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.fehbvm.com/Article/details/guqemxdln.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.zdbjq.cn/Article/details/gebxuclwl.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gcmurtkbq.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.fehbvm.com/Article/details/ghaeellqw.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/gomynvuvl.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.hesvh.cn/Article/details/gushssmkt.sHtML


<!-- 参考信息 -->