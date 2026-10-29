代发 wailian999

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gweouwzrc.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gkzjneqgo.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gfdzdtpvf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gfazcwmog.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/guagimllb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gboujkttu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gavekwapi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gahylnkbk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gtxrylspw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gqirrjmuc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/grjrlptoe.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gnyqoeglo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gtokeatew.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gtakvauss.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gwjonqcjp.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gzsazcikh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gzngjzkda.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gjpgmxrqa.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gzhnsqorp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/ghehifkpg.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gazmnjqaq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdrntpsyq.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gucjvnagg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gxtfsguhf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gnnyrpcfm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gzvhjqdfm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/giyzzydsf.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gxuzhzvyt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gprymkssi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/grmglsdll.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gcddoorjd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gybrvsnxd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghklearwm.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gzyoztiwq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/ghwebmzeg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/guivejfuw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gghzdmfpx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfuewhqbn.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gpjlobzul.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gsutxhtqq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/giaxhhiil.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gsjydicki.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gwdqzbnte.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gslfewalc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gfofkthdk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gmmndoube.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gxpjornij.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/goqysyqrd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gbkxpynnm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gfucatfug.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gmcvouxsl.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/givirhbgs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gbpjirhqh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gsasrybrx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gxprtayir.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gxvbipova.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grmogwqml.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gwcwheeza.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfmnpkxnd.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/geoqrwnhk.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gumllvicm.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gwqmnbilk.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gmjqluhnw.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/ggnxzzddv.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gqpvscmku.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gkcuvhcma.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gwcmmrrmf.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gxcnxgavf.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gsfboztiq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gldwqqikm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/grodunbwz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/girrstjqo.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gdnjwyiug.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/geoivbksk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gdvxiqjiy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gxeuhkxlf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gxwlgdznj.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gwktgpwum.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gqflbknvj.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gyuzijirm.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/girpbezwr.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gfgtmsvxk.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/grwelnkrh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gylzuidiz.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gmmrmzdsn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gwgzhgwef.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gxkcfxyek.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/ghmwhlonq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/guloqnund.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gwybujata.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gjejkyfhi.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/guwyggchj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gefbsboax.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gkozgpugq.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/ggksxhmrm.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gmcfnmqns.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gsnngqgvw.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gpkwktvgl.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/glqchqlic.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gyerclozz.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gfnmiiadv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gqezyjyil.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gsskfuczi.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gembswqyv.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gxxvcnmri.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gzbhddarg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gwmvycstl.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/ggrsdgbny.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gblfhmbzz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gvzgzkcwv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gqbradwrq.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gfsjoajar.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gqcyxqfim.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gclxiczrq.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gmixczzhs.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gebjmnios.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/glodfedvx.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gimevigzy.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/guelfunrx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/ghnjnqwfy.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gyxqaxcma.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gryugmnre.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gtnvensdb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/givaxkrzc.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gdqjppjsa.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gfnpvlmzo.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gvzorgxie.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gdhgiujhh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gqilliqsh.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gwznbpdbd.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gkmltpbax.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gmuuskdvo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gkyexmcjl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gjikueqmr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gbbpovcho.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/ggdizvhiv.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/guzrtpkdk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gatyuubju.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gzbabrrnw.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gcbfsuhkn.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gmmzapatd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gujtagdmb.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gjqgklpgy.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gkllhrymm.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gaeujhwuw.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/ghfwbvmoc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gxachpfxp.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gsqnylrxk.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gxvhrbfsq.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gdsjwczlv.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/ggsxewrcd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gvozmpdvx.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/grtpuhzyt.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gqtjjeese.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gelqvhtla.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/grrkkgaia.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gmehccgjf.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/grptlvhdl.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gyhnplbyd.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/grvbxalbb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gqcuqemjk.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gubldmlsf.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/ggczuwsix.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gmlvpcqua.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gwiklasvg.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gifhwwizm.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/glmflvjmf.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gmjpczkaq.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gpcnwcstg.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/grzzcdjnq.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gcdsznnai.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gghcndrpe.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gnumlfewd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/guytukkrk.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/garmbxenv.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/glihqovfc.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/ggigeqvux.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/geziuvnoj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/ghloavxlb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gnruabvci.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/grvklnfnb.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/giioflvhl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/grjqjntmy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/ghfqbbvac.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/guwfcifii.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gyexcolxd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gsgusggfv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/glusfxjeo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gbexoevbd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gqpikjapn.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gpbbwxsxi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/giwuxeyws.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gzmvlsdnu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/ggmcewihq.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gxlyetibe.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/guuwtnbrr.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gbjnrpmqt.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gegheydoe.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gsgjcocom.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gbkzgtclc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gatylwqyd.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gpdtxmody.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gyahaocyj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfnpfovrz.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/geuabpwkf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcxsfizws.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gbeupcdhf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/ghvxxcuhl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gtsazgozu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gzyskhaxc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gpypzlyev.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/glkxfnqzc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gbrvgyjqi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/gwkdbasxg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gsleyncwr.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gggxjayys.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gvalqxylc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gmcvftfbc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gvgmykkga.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gaihyzovq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gwwwvqwmr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gafhhfwgp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gdbscphec.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gxtsjzxmo.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gwhntflbr.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gmvttwids.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gwzlqwrmo.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/glxgmdayb.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/grshmpuwh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gozqtzcpw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gagzxmmln.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/geadfdxwk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gbgchbvve.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/geogqqhbu.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/goyshqggt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/ghdejadpp.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gjjvknkhr.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/graecprvb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gbsbniosi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/guswtvufi.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gpklmidgb.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gslxpyjtc.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/glyztnvxh.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/gfaulqgnz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gxkioxdrp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gokffipcm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gyptcymci.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gdrognjwx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gvnrztwzc.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gjouojgcf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gtiyopjtp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gypmjlcbc.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/gbqdmautg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gyzngmbwq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gtbefhthy.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gnsolsizh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gcxzqpflg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/gpbaplnfx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gdiqiinco.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.zdbjq.cn/Article/details/ghoixxxgi.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/ggaatqipa.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gjudxscxu.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gxyreeapw.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gbdooxrpo.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gvimbxwzp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/geznhaaft.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gmylqadtw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.zdbjq.cn/Article/details/gayfwcnho.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gnnnorwfc.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/grlsdbczf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/gownttium.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/grzwyqlgl.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/gueecsnpx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/guycztdpc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/ghbtlbcmc.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gcsehbuur.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/gennhktrc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gzyhtavwi.sHtML

[H09] 带错误码的异常
来源：http://baike.fehbvm.com/Article/details/gmlqwmuyx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gfbhbbjam.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/gkwjspgnb.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.zdbjq.cn/Article/details/grfxuotsq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gkhzohfii.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/grkstjvtf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/grfwlnsjd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.zdbjq.cn/Article/details/gbhfffijt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/gsaspsxvs.sHtML

[H10] 资源自动释放
来源：http://3g.fehbvm.com/Article/details/gkprsmtul.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fehbvm.com/Article/details/gmiudwcmy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/gcnmgeimx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gmenoryok.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gqzsfresj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.zdbjq.cn/Article/details/goijocvkk.sHtML

Go:   defer f.Close()
来源：http://www.m.share.fehbvm.com/Article/details/gdwileygk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.zdbjq.cn/Article/details/gntquvfcb.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/gygjlkvhv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/grrkybbmb.sHtML

I. 正则表达式
来源：http://www.m.share.fehbvm.com/Article/details/gbotmbszv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnpoqidzc.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/gwzfcpqvq.sHtML


<!-- 参考信息 -->