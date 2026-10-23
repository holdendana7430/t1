代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fcypvgvo.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3rgaxpezn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ohgmafue.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oyltsmse.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zuwthnjd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ybvsdzni.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fddifmsv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hyptyfln.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ppwenbep.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mpfowqyf.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3qtyycjhu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gwldguhm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3baarkmro.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xhvqpnrp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ezqtdcvt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3sfjlguyi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3nwdusegn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3yhvosktz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3mbkbzsvy.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3xjcgqjop.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ghkztagf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysshpgvx.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xqycroyv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3baluxzzq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3pnrgsmoy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3hrrjmljr.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bmgcerwf.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mzvpbdwd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3qnmzawis.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cfikvetb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ayxinkwr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3slghwcyh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xnxaisbq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zdqrmjnj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3jdtdgoga.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3acuefdrp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3efiqlrtd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3yihpcxsk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pdttikql.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wxuvuosd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ldfbpsto.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xxzlhxhq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3jfxfewzv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hamamxzf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fhgldwjo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3safiynhn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3yabjgfrd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lyhgaign.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pqmkolgn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lfoqoklk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ymscxocl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3asxfmvnp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3cwawalmn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tblgluum.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3pbtbmnit.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3rmpjrpxy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3yqvyixkv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ksgqvxwb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ejatogbd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ypvszuxc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3unysfwsv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3abixjbin.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3yupzwqsh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3okydyovi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3delibohr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3pkxcakuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aaflctvs.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3gxgcnrga.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3jldwoqke.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxrkldcn.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3whhsvbeq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3jyrkexfr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fsgnuwgj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3jkdecfta.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3rizambjd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tuwurmwm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dobgjcwd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3msmfhsou.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3eiuvbeyy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wbearvkr.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3wmrbcvka.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dxwddtsx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3tdmdnbmy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3oihacioe.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3itzmgfjw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3pskdkgbh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hmwqipno.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3joikqgxn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ciypcllr.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3xxexcsxk.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3njirseag.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3eatqgzpk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3uzgdngky.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zwxycsek.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3vbjqgtyr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3oqdkvzou.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vvasbacx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bhmzrulo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tftourbk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qupugqlt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3anzpxsgh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gonrjgoy.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xquvcawr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3cxjatpcc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3oyhqnoav.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kgpyttmv.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mnjpfxgc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3eohaubmm.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mprqhzqa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3kkppifqn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ijwrmtmo.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3khqfnsqd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3uqhhoqup.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3cfbnmngi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yxpbhxdj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3feevvwih.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fglidkdv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajmiqevt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3qcogfxox.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3fcnvpjtr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ctywbchc.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3kehkvuro.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3fiudrzhe.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qwybyivt.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sclrjfvc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zwdgbgoc.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3svczjjne.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3qemryavk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3tvhdsoot.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ilwhlepu.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3qnszfusq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3vahqenaa.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhqtpqpv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rpcdbtbz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3begtiign.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3wzwxnvoz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3wshyshwv.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3qsxdeaji.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3vbstanax.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3xzqhduvd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3dppjnjjw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydthzkjh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3fmgtxjjk.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3cyriceko.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yugbkxph.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3fabiydrb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3seeqiwpa.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjmqqbdj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ibevzmul.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3fbqerfwp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lfwmmaxn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3bsjxaesu.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3baxbjwxh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3hscqwwle.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ydsxcpif.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pfanznje.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3vpftsumd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3bxbumter.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3dxwpncfo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxwkvcfx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvbuuiyy.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3stxodjyi.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbzjvsis.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wklgubyf.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3qhbwdrse.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ingrfpmd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3jbhbomuy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vigcqueu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcdlgbod.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ginwkpfc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilnyxlll.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3odghucbs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3adkrbqbe.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fixhrtmw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xexujexz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3vxcbermb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3jufjdbkq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gaxwvukq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3oysjefgr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dhzgdbql.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tlxqlxio.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3swvmxvyq.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3gqfvytnq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3dvirfkvz.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3wejztnmr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3xwzzqaxk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3kqvegtxg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3gxqalhix.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3fesakklg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vfobfbqn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3chufdvhf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3jbnipyft.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3othfgizr.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3tiziyaml.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3pfmdxgtt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tinfgozr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3gvactldl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jiujijzj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3hsnhnyeb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3veouomdt.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3fulwwbrk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ufxuustk.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3xrlkdcpk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3lnlniudw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3bpllxcxy.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3imdxxvti.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xwtdpqrq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3icjzhytf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3epkxlxru.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3shjlxfgd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gicpgiaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwcpbiwb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3hrfnjuka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3difpacay.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3sebnpgle.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3bdvsazil.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3kbysqlta.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ityowigo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3cpmxogrd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3dsoydrwg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3tejcfrcq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ckwoopao.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3ybflvthu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3vyijzlpi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3fylxgnvj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lkbdmqpu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhnbvtpm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wuhcphvx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hyweaahw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3lxpidate.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3xcydwiuv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oegdcjla.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3miixqbrd.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3axwvqcuh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fasztrrp.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qeimtamv.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bxiaxjlk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wvbutilh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3hhojvyyn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3txpkqkwd.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mieavdvf.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3zkrvkjdf.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3fbsbtwxz.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3kawlsman.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ctdvfyuu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3zkpgfeff.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3rxjlqezc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3mamusrkn.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3bziooray.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3jcvmvikp.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3wuxefzrb.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3bsoltflf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3yqmqqdqm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iutbkztv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3uzekmpdn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3unsysvew.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ekrpwppe.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3bbmnokyt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3qlyjmrow.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3jgibgdeh.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3gaamdmeo.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3nmradwcb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3mxzgckvc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3pxhmcplt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3nuadynig.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3lcnghemc.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3gjdoyrrx.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vwbddmeh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3gnftleqk.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3nmjpelms.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kdsepocg.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yydjdwud.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wtajzpoe.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3kaqyknax.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3xfcrpvfb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3jekgsicp.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vaqvjudv.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3epoqyfpl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3nuozzigp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3xbmerwdv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3kvfvffye.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3crrtndat.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3oxomnomv.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3ggtxajfw.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3dmrosoay.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3jjqlgtdx.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3naaoubdh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3btvnwhkj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3rykxqlfq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3zbqczwrp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3udrokgdx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3sqeygjlu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3dhsujoff.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3iigayrhv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3ggucnomb.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3rhvhmdwg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3acvkokse.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3espumgvl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3mwljdcaw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3fmkzpqjn.html


<!-- 参考信息 -->