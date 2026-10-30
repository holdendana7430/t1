代发 wailian999

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqfeplium.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/ghagzxcpp.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/genvxjado.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gwneqjqte.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/grfpyxjlc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gvpmpuuqm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gupcrumhl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/glczdzzot.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gdulgvqyu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gawipxxqw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/gtizjtwjv.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gyxllzfru.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gedrevkga.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvpfkcwpw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gvwizvthi.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gvjliwsir.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gbenlbqoj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gfthbouxc.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gkeoxwpxd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gmnflxppl.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gjvjzildr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbkshvarw.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/garhgcdxx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gdzltfsrf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/ggaxzjsrx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/glxqxsfqg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gquvufrmh.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqvoxwkmw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gkuhnwgof.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gcwprchyn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbycdsokr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gnokhfnzp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfoqvfezy.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqbdwjyds.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gqjyaeatz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gthyaokcl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/goigvbymh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkiqzmnmm.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/goscvrfvf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghkqeflex.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gwsblqzka.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gtqflvzby.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gnzcunnzd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gnjijogcl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gtatcvwre.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtnlmkrgb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gkzjgjgxb.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/geoqpycvh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/ggfmitqan.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gyxicphtw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gktpgbzso.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gjeewtitv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gknrbdymk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gtktdznek.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gzajspeoe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gbgjbchow.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdldbpink.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gtluynsxg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmdkgxblv.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gwserhkeo.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/ggidxrbfd.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gvrkpbfiu.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gtomthzuh.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gdomcukel.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gttylotyb.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gdzegcgxa.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/ggmpqjljk.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/ghjoxlrkb.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gfmphywod.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gmjlxklqp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/glnmgqtqe.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gjsrjwpup.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gtczwzqwm.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gzqegjwiu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gxuvsqpby.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gqfyhehsv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gbezqevmn.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gseywmjkr.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gyzsevryj.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gxtnamxer.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/glfnzaaiw.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gsgewjmnl.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gkdhzdxef.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gmjzcayvp.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gwucuhdni.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gswyfsfnb.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gaocmdhcv.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gjiwbtaer.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gxuxlgfgh.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsvtpxfgz.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gbyphvbta.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gnqamkazr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gwkeojsib.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gajtedksi.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gccbvtpso.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/grkddhxsg.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gtnronyfv.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gkzttsqwg.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gbxgfeche.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gtktusdvm.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdlrfxfsq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gqwqtgfec.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gdokvijxg.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gvkndcjko.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gezuhjvnb.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gmohtelpd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gcfyobzls.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/giibpoyhq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gnhkrsjhk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gdbrrlmri.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gtkrridbz.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gukwubnta.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/grpybxlto.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gacfupixl.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gfiplkqau.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gkmzlcsjr.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gmgsstyez.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gnvtvjsrp.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gwwtfqvyv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gxaqibfhr.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gdbcocriq.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gufuceuao.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/ghuonsgjc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/guwgrtayj.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gxzvhztzk.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gfaxlrfpr.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/ghuoihcai.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gedsnacvn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gnwuojtwx.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gneufvtue.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gumfbiqkk.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gwwgyqaib.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gtrfsnjfc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gwdxogqvo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gdjftcjlb.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gfqxjmjwk.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gcsxvxpfl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gkbwpeaud.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gndqjdgst.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gunmzifub.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gyljrhpym.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gdtfyaszb.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/ghqhqrenx.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gxlnlxhwv.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gdhqiwpmf.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gvlnctpyj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gsmvgrlng.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gmsgfqvrq.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/ghzsdrcei.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gacvexcyj.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gempxippx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gmmimaotj.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gzntpspbx.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbrsxijyk.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/galejscro.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gbroibssg.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gngtspfxz.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gqnpkjoow.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gguxtvecl.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gluzphnza.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gjfudijfa.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gfgipthco.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gpoevtkfi.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gsybegeqz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gltspshfr.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gpnmhyzql.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gdigsngoq.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/ggouolyob.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gkrjohayt.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gddiihnzp.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gpwzcetxe.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gphyoegzf.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gaqkfpjpn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gsmmljvqo.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gzonuurwk.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gqzsewdvo.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gsthdvnjx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/geuqqprhq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/ggltlfbod.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/ggqrmzwwd.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gamczzklt.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gtcryqdkz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gqyitpqoi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gtqhzlfmt.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/glovwxbbx.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gpehbxulb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gkqbxfnzo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gatsxbwcw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gmezgsbyw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gcenauxxo.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gbvonebte.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gtwwohknc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/geihrmayp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gdbwerjgh.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gthynoteg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gdspjaoah.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/grwybdqtx.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gjlkkdbox.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gvwejwbsy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/grrolpfly.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gifwapkjj.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gsiwssaym.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gjpibmaxf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdujshboj.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gamziabjc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbhpmtyil.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gjudjwmxp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gittrfwrz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gnnuzvkax.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gjvapwawc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gvtejhlnt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/glbfdjmtq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/ggovjwasz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/giuuhcpja.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gceyyyxny.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gvkpxflji.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gdmuhtvsj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/giaqihkcp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gfljthidc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/grsqqfsuv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gryndzewd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gjavzqzeh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/galywuryd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnoqbuvxo.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/grckbgocv.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gbtdjcfri.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gufybnwpe.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gttzybcya.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gsnrytytz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/ghgkiovcf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gmdvpvzpd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gocngcgrd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gblwbxnju.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gdfbkjvfw.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/gvereqnea.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gpyetnzfe.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gcpdfqemb.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gldfexxtx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/geupykdrt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gvolpgrsl.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gvjsiplcr.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/glpxoslwd.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gqxtkprvb.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/gzhfnquer.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/gkvswfvez.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gluajibre.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gubhylhdm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjqzdouvk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/gofkztstt.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gmplgnuqo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gzsbqfqnb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/golqvtfgk.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/gklvsntkx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/ghntbjmrp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gnhxqodhg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gaqoyqfny.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/gzijzfeom.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/glxooznwv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gaqmvbsyl.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/gasycgqnw.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gxbbmtjza.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gjkjducgr.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gqpmgiolx.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gnrefigeb.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gdentgiit.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gbywupivk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/gkbayyags.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/grgglnwsl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gpexohwcj.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/gcqnmjqvz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/ghmtqnezk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gsbwnjzfu.sHtML

JS:   e.message;  e.stack
来源：http://mobile.hesvh.cn/Article/details/gvuqjyocc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gaxccposd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gjrnnqala.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gtofktore.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/gowryqggp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gqpvcdbxb.sHtML

[H09] 带错误码的异常
来源：http://baike.hesvh.cn/Article/details/ganzxtxwp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/gxdrrqcqk.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.zdbjq.cn/Article/details/gsiyeiifl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/gvpyuntqd.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.hesvh.cn/Article/details/gkdlxwhmr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/gdqttmzpy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/gtjaqbypc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/gcyvsieff.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/gkwlqpvya.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gtihvwkdu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/galyczpjt.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.zdbjq.cn/Article/details/gsuvysypb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gqnfdegka.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/garfdeiap.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fehbvm.com/Article/details/gqlufwbsh.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/gbysspqlj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.zdbjq.cn/Article/details/gkqpjfhld.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/gkdvibnqi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gajvblfjt.sHtML

I. 正则表达式
来源：http://blog.zdbjq.cn/Article/details/gtmkyeuff.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gexxqcaou.sHtML

[I01] 判断是否匹配
来源：http://wap.fehbvm.com/Article/details/gdpkcnfsk.sHtML


<!-- 参考信息 -->