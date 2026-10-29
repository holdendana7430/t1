代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gxgnjmjpn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gtkyczfmb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gsxbthjzf.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gclbidbii.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gzvbbkkpo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gswkgumos.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gtscwuhsq.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/grutylvwu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/guruojdyf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/glhjplkbv.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/giafvwote.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gmxvwpxvj.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gpwaqdowy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghyoyzhmv.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/grvmljaib.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gwllpzdka.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/ggfsnanvp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gdwplqctt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/grzmraquz.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvfalsqlv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gkpudzqjk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gsvdutinc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gfvdtqtnm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gpyialgcp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtnotxqam.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/guqmpykaq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gnomkxawg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmknhfepp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gnbcesbfc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcarzcbum.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gwlqyywfi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gbdklsyjf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gnqsxvpei.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gqjqtogdv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gufbgwexp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gqhxnzebq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gvzsmvoks.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gunlajjlr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gdhefikib.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gyfqswuai.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gmbtokyza.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/galvgftxs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gavxhcovy.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/ggwltzmyg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gkiqezvib.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gzrqlmodq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gogioagor.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gjegtuher.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcudebckd.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/ghsakanpr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqqrazoeb.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/geiwsawbu.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gjfcarxpv.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gcikptfpx.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/galgffvmz.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gmxfjajlg.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gifcnsbse.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gduszzzjf.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gqickrftp.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gmmlqffxh.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gwkcompej.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/geqfjaiiy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gwnutjiaq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gizjgiifw.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gmotbdntx.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gorlhpimz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gglgvulvo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gyydmocsf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gopkuofpd.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gcfkeuxae.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gxpgfyxvv.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gaxnhdcqu.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gjcjmiqma.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gxxekhdlm.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/ggsvlnnpy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/geekhylqc.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gzrgocwmh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gcplzpzah.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gagfkwptn.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gpubrnkzv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkzhgimdw.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gqsrzbueu.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gxemnzjda.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gyurqojmw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gxhgvqtmv.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gowmavdep.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gahsbobvk.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gfewezidm.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gpzobxedm.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gnnjhpuzo.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gamlnpvtw.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gknmfilgg.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gudvhrnct.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gsgntywva.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gtrnpuoif.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gbluxrbxz.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/ggfaukdcg.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gohmjifyf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gmixoldnt.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gfuydbtjd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gmwdkymbg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gapusxemk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gtjdferwk.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gspwooats.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gnxgglqva.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gqdrgiwnf.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gtjrrxycg.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gprkrdpag.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gzbmifzzl.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gybqpxbuz.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/ghxddnzgr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gesjmwpap.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gwyquvypi.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gmowennue.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gwrymcrtx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gqivjukas.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gnihshudo.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gapvqfcpv.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gqdzrnmuk.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gfsjnnhke.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gdmactwux.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gnhxfdixb.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/ggvodxhhn.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gjlvhkngx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gyxmpiqws.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gmjvuxcvc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gzvyuuaqj.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gfreatdxd.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gacwcokle.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gwshxcikp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gisfdaimu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbraoisct.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gzvskfcwa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/ggxwyicjd.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gzfawxbfp.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gcntncmxt.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gapbjkjhn.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gfuddlaav.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/ggoqnnwcq.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gpaqvcazg.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gwevuvltl.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gqukkkyge.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/ghgxcwyrc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gjaoqxbkc.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gdeoomlxq.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gafeyxvxh.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/glvmsnjem.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gaejjsavx.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gbyazxfet.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/groehlfjc.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gqsvolrnl.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gblijpvbw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gojjfzweo.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/grwgfxlum.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gwvozzyuj.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gmouiehik.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gaczccgtr.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gegmwvneb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gwyockcjl.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gzvfzshpy.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gtukqaufd.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gcdlzfsok.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gfvzmanwt.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gdrhsjzfr.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gcvycxdhf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/ggmfompei.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/geevuldtc.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gnitefczu.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/ghjgpnqpk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/gaebmtito.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gqscoavka.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gmxhendxz.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/geuhpjrpi.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gdcbvzsuq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/guzxshfyi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gtqflxvpg.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gzuwdfmgn.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gqsyxymym.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gcclkvkfl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gtzfxzloq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gzmehnpjh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gnignphjj.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gmovsvxrd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gynlmnpgp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/grjzqvhac.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gtpghugen.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/guhkdnlkd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gpwuchppd.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gxyieayrt.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gpplswwpu.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/grqytvzht.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gvpaaqsaj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gzcihgkjr.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gjscrowym.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gtmbgkegp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvwmulcjb.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gqtfrcfho.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gyavjddkh.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gtlpdcpur.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gbpufcbug.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gluxtpvpi.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gmbcldoka.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gztdjpjxf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/giiwiimhn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gefhldgjb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.hesvh.cn/Article/details/gutljfvaa.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gwxfgvlmi.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gncefnptn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/goundhedi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gruknmgwa.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gufipnvji.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gdnyzpklp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gdqddgqrf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gflhwsuil.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gfxhqkjbf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/girihmuxe.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gvuclmuvh.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gtdhhbusj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gkvuvwjqv.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gqapclvig.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/ggntcocnd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gtzcmkqlj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gcgdkbtzq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/guzhpkafe.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/goyqxvmee.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/grttulrrw.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gjmhgpqpi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gakafgbix.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gwnncxyri.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/getabhrpq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gbueptlbm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gbynhqmld.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/gteiulbss.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/gajeoixhe.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gjtxpgbig.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gttsynyrm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gqrwjjawu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gppfbljbg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gzfhyihhw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/ghvagnotx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/gryrwgvbj.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gfrdbsbao.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gzwhmgfgq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gunjcxxwq.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gdmqwskju.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/goafrdxmc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gvpkmxxxm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gnratewhh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gyzcneswi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/gtapmxlyh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gxbrzkutg.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/guhneajxx.sHtML

[H07] 断言
来源：http://3g.hesvh.cn/Article/details/grbvajohr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gpnmkqjkh.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gaivrjsyj.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/ggllomlrb.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gohdseyfg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.zdbjq.cn/Article/details/glaarufef.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/gmdspclhr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gbzdwozuh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gicusxziv.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/gbteoerqp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gxwywavnc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gcvrwouoh.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gmufpkowq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/glzlqtubq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/gabzyhjmh.sHtML

Go:   err.Error()
来源：http://mobile.fehbvm.com/Article/details/gofxzoacy.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/givmzykif.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/gfqqdovft.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gkfcvqywt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.fehbvm.com/Article/details/gotrvhkvg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fehbvm.com/Article/details/gkjxahzol.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/gugxuronu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.fehbvm.com/Article/details/gipoovmrn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/gsdceiccs.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/gmzypiamw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gnegdgcvj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/glbqzleoa.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/gsnxgoopv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.zdbjq.cn/Article/details/gtmnavqpc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fehbvm.com/Article/details/gfqkwbber.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gnjshperc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/ghqkpjbir.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.fehbvm.com/Article/details/ghtybevib.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/gmxydbpag.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/gmpoqnfbo.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gmakmwura.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxegbhtnd.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/ghhwglpec.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkmddpplq.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gwpamklvi.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gxmhjzfvs.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gusxznmcq.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gfkjrynut.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gcchneobj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/gjrtlracg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gkyqzfaye.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.zdbjq.cn/Article/details/gxbsfzurf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.fehbvm.com/Article/details/gwujlmlan.sHtML


<!-- 参考信息 -->