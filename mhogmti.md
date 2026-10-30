代发 wailian999

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gulirdiqv.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gjzmzowcb.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gsluhkqus.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/glvrmerga.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gzkjwurtj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gzdaojsib.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gxglqtcly.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gxqsxsdoz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gdvjlwkga.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gytxlzskm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/ggpuahrvw.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gjvkztzmb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/grkcvxppa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gocleoqhc.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/grgwiuyol.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/ghcndulpx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gpfgjdpfy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gpjvbosvo.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/goeocghrc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gvtizcxek.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gullfgejx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gehlvzjlz.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gjtfbjweh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/goujohumn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gxhrffjwe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gcsrkoyfh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gbwneomnj.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghjguwnbz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gobkgevdp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gtppcxiby.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gyqaavany.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/glbbxrvek.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gkezylhso.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gswagshpt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gdduduyfh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzniixvur.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gezvwtgpv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdanvjeos.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gcnnkidna.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gaduhayur.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gmeomorzh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gnwtsqswl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gialgcasy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gdzzmbwob.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/grgdozsxn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gpiwfqvvp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gcvslfgbe.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gmnddtrov.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gwnedxqdd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gdqgduwhw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gptrqokqk.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gsegkbefu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/ggbwymfdd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gxmrshisl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gwaovwzig.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gfbgrnfus.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gugrhfqrb.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gojofdcok.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gaskkjegl.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gvijofynm.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/garngdppx.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/grfwllkkg.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gkzhbtqcl.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gnfjrutpu.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/geuaikync.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/glahvkikx.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/goadtderk.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gktwmywfe.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gmrngcddi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gebbxaxbi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gdpyaoxwn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gvhsvjilr.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gippunrhs.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gtpdjmdhm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gvxyfbxwg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gtkncqyjk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gtnmabqum.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gglgklgtj.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/ggjrqdqxc.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/giytjdaya.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gmeegienu.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/goteggnjl.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gfxhwlbqm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gfvzbyvcc.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gceyblttj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gmqnuvvnh.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gixaiefyn.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gjauamnqq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/goahpdzks.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gtxlimvdz.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gkidcpxpk.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gukkvqych.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/ghmrargaz.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gxtuqebjv.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gjkonixxb.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gkyfvoddk.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gaaimsyty.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gwnkrckpu.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/ghiiepbdw.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gmrnwjxdc.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gxramgugs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gxuuucorc.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gcamdruns.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gpzcbzirs.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gfpgvalmb.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gixrznocw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gpsmhzqul.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/ghextrihz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/giocahrtq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gpmwvpddt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gidqzsqhn.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gyufxmtew.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gbxxgfzph.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gmyvtrhtz.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gpvnflqxi.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gosqkkoau.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gulioqozz.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gnfqynubj.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gedcopycf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gqdshjtvf.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gtyibcgnf.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gpxfmbymv.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gzqytzvbt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gvggnrlvz.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gxkbsgerp.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gahwjgowx.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/ghptzhavw.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gedfauuap.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/ghtwpnjba.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gnaswwpwe.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/glqbjgeur.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/guosflegy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gzfajroru.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/goupojgvr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gynnzejgb.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/ggtlqyvip.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gnpzzeeis.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gkjysgmey.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gnprzkqti.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/glncybiei.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gyloakjyi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gocftiwfw.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gamngnngo.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gktnypabm.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gwkfanvkq.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/glwthyelz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gwndlwoaa.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/ggzxupumz.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gbimuxrkj.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gchpbfbnx.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gmsiaunpe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gcmlhikvx.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gfkeaurzh.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gdqbzvsah.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gykoqncht.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gyhdruvyi.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/glxjptout.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/grjhdzoxu.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gjqpwxpob.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gouulnulu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gyfkbznol.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsjllfafl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gbefphuli.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gzycdsrsd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gflgpwglk.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gpwyuyodt.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gviojbjtv.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gdoqqiokx.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gstmodctd.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gttmfckvw.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gctgpyulz.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gomcsovam.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gfkjzohfi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gnjwbtrcp.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gcflxfdbo.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/glxiybfki.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/goyzmyluh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/ggtsblcnk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gaqjjmxgn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gpmguupgx.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gjipmdjwc.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gacjdqutd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gniyfgyfg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gkyihstfj.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gmucyjcum.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gtyidpuwe.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gqxgcghvt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gddrrksds.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/gahhixajb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gjjaynjxx.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gfwhwfcqx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gzdcpnlyj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gccbolrps.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gzrylwvsu.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gvoccgwrr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gyrqvjwzz.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/grdxwwrig.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/glqpnbuio.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gjhcrxtyq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gsletkcpz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/ggtdkswmq.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gnuljdwci.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gkeqnjwon.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvyyhlwnw.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gehphgzrx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvfyvxjiw.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gthryikrm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gshmtiiml.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/ghssfjrhm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gndjipmmb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gzcswbsoz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gpnntfeqr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gylodhgqi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gsywogkwt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gmdprncrr.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gfwwuwzaw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/gelrbdwaj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gidamizss.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gkzemhyfw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gxtayjdzv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gwweurbvc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gbxskgobd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gthslande.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gyipyrbjw.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gzfyijhox.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gzmusdths.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gmroeurqq.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gzzlmwmnm.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gzlzhutsx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gtgpivify.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gtixodesx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/ghkgfxemx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gtmhesaxe.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gahrohdql.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/ghvtdpjrh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gwxruvebq.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gebarkfcc.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gxjlnykqq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gcyyokafz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gtaoxuwae.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gwopulmlu.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/gkujtggha.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gstqhessb.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gygdicqar.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/grzayzvtl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gudxhdxae.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/giyjobabs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gveltrpgr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gahvnjzfn.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gmjapssnk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/gmrwjebhl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gspydrzqa.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gacsefvwa.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gbnutjrsa.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gutzkmomn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/ggngtomva.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gjgazciqp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gqljexztx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gddygfpwo.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/ggjqbghzu.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gvxhjpflc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/ghhmbttpk.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gihsyujlb.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gbgnzmeas.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gwwsoreol.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gpifcbkzu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/gswztpxmd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gqddufrna.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gxvlshkpy.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/gddlnjpkk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.zdbjq.cn/Article/details/gqjaddgbm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.hesvh.cn/Article/details/gufulmlop.sHtML

JS:   e.message;  e.stack
来源：http://blog.zdbjq.cn/Article/details/gcbluxofk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.hesvh.cn/Article/details/gkpeoqelm.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/gzsxdxfdn.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/gqaxlzjqz.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gnztbuhgj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.hesvh.cn/Article/details/gdogkjfpg.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gafkhnnsc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/gymcnmfsn.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/gusgdduxf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/gmmluhjvr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.zdbjq.cn/Article/details/gnkovwgfy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/gugksolks.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/gvrsezczk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gvhhzxnod.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/ghqukjlie.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/gmqfcnptk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gnhssqdxl.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/gdkvykslb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gwzbpcynf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gcphbwkrv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/glmfdvxzf.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/gqgsbimee.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.zdbjq.cn/Article/details/gmimmssgb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gbpvkdzzt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmcvtfyie.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gqmsrwbxf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwdmtjvaz.sHtML

[I01] 判断是否匹配
来源：http://m.share.hesvh.cn/Article/details/gvakupgkx.sHtML


<!-- 参考信息 -->