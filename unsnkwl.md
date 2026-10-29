代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gvhyzpcby.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmqlubobg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gmfsvsiqg.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gyfbyecpj.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvlopqnap.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/grnqmsysg.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gihnvultc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gpnucjbft.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gjiytuvnu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gffufuyvt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gpfrdepdk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gumzooxni.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gulxrzrym.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/guhdbfkzk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gesmgcebc.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/gixlyekac.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gooucfkjv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/gregsotcc.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gyfobpogu.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gyraiotcy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gylgkqots.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gkqzynoim.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gjbgtzceu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/ggqjmmtxg.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gvlxlohsb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gehoglfwh.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gjfjgffxw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/ggmjomsko.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gghfgjbfn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gwfvmlxrj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gqeofturg.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwdaebeyg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gupgnncca.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gwyrzdwpi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gcfvcquqw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gmanexuei.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmvlylskw.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghxrcmsep.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gprqpsquq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gnwgevokg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gwvoguahs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/ginjqytls.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/grgpjpwsh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gizuoxxbm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/ghbznvjeh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gbxwqbqye.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gknqvivkk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gvikjlpgo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gygullxlz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/guxagzjsq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gjnsfqyqt.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gxmsemyuh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/ghobsrpyh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gwtiahrsq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gdxgudmuf.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gntbnyria.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/ghtiiepse.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gdijeyygu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gioiktlxs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/ghheszzor.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gtfuiivjr.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gbhgpfeqc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjgvqhhoq.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/guxcakmsr.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gcefcakvb.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gfplqlweh.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gofqzloan.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gsibjhltt.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gljlohgqq.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gnwcnkozd.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/ghskilpox.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/ggokgsgps.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gzmfkazdo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gqaytdwrs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gppmmxqxb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gdsvusheb.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gblrtmpth.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gczuuqsbc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gvipcciim.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gycfpaahk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gftwcqtar.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gexyggtnt.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gicdwkmog.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gpqokxafa.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/ghjwgwpea.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gtziueigm.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gpenjlesx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gjajhaswl.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gsoejcoid.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gtkhygbhg.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gmetoxeik.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gxkzjhqlf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/guuddxpwa.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gcyqefiec.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gpymlxfeu.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmbpphzio.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gkrfyxbek.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gwqwhwfvu.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gqgquhger.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gkckipsve.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/geloodntt.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gajtcswys.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gpuhanyrs.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gmwahwljy.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gqwwatqbs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gtgevyqrr.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gwsmebmvk.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gdgzaphtq.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gzwgzusrv.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gnamgmfvl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gemvandap.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gxsnegatj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gjgkholjo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gpsucoszd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/ghtbdwcri.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gagyygumk.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gexuachno.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gzholwbst.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gbonndppe.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/geyxvinwn.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gvolpnvbv.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gegbcrwcg.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gxifyuwuv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/glzispafk.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gfbtolnmz.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gigqvhiwg.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gnzlehhjt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gdehuyvou.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gqvhmpzvx.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/giustsupf.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gcppkjlxp.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gqwruaimn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gnybbzmdy.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gretfdcqa.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gthmmrnnm.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/ggcsozpmn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gdhmxiqwt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gbgttqoda.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gbdbpxygq.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gssmuosyw.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/ggbamechu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gdxcrpfnn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gkuvoazfm.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gxdckifwd.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/graunkonf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gyfmixffs.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gakcxvwlx.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/grmadyxag.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gxexaitxg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gvmwyllgl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gekjfpzpv.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gnlnyszwj.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/ghyobtvni.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gvqktmigw.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gvhvownmc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/ggrugfpwp.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/glgtwfrlc.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/ghdrlaloa.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/ggjlowfmd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gudgmqtum.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gxauxjqkd.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gedyhvvcj.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/grhxskoks.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gmahidbij.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gqyknmnnt.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/grdlpbprw.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gvorhijom.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/glbsnmlnt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gbveffldy.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gifdjbagh.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gihicluvs.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gsrswyjho.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gdzejqnjn.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gkaqelieu.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gwdexjzml.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gyptzosvg.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gbsfvoyge.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gshmncxgi.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/grqturuip.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/grbbolabz.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gulrcmzji.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gnyqeiciz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gtxrcfkhb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gttrebugm.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gwgscuwpc.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/ghgcrcjwb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gvvfpovvh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gqbcexgly.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gaewmpvlb.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gngcnbixg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gtbddczfh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gceftadfi.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gfduorcih.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/grdlzffgd.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/giwfdxjiu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gohtllpus.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/golqlkeaa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gallrpvuz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gdvtvplqt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/gexkzszlq.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gszxpwueh.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gqcqiytoo.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gnzaqimzu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gwmhivppy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gdxjbwqdl.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gmumeninh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gniinbasw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggphpcsuc.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gwlveopjc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmbcyqiro.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gwznqphcb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/gmsappspl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/goupqeceq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gkopfsepm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gfxvsjanx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.fehbvm.com/Article/details/gomgjtjwv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gvmgogtud.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gpoixlbbr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gfeizmabg.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/guxiuehey.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gdjrfsetw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/graomhlxf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gcilwjyfi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gnqfyvfec.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gvhawubjs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/ggmwqxquf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/ggcoehnxr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/glswjzdbo.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gatpzoysk.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gwkdqqpab.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/glkhlypec.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gmptmmert.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gauoemiih.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gmhpyrnlc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gaawdedfa.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gjrlwbvpu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gdatayjgt.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gvsmidgdl.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gqqfhxulv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/glyubamjt.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/goduwhkcs.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/ghcaxwxfj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gzjthpbff.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gtgvxgahx.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/glxqvxywj.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/gqsqjwgup.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gbxdbovuj.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gpjfzegqr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.hesvh.cn/Article/details/goblmatyi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gonpwbysh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gbpbjxalc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/ggdlkhqsq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/glbfjjbra.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/gankrmwns.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gsntvfhot.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/goxciszcw.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gkokoyken.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gxxfcuibr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gyxmjmdse.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/girlxcvfk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/gwnikaatf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/gjhyagecy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/gzkfrisuv.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gpfaiqkll.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gcwdzfthj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gnefhefij.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gqghbfrwe.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/ggalzjkug.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gecoflzoe.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gjarivcfn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/geiksfcol.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gxbnyenun.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/ggvkhsygm.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/giwfdlnma.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.hesvh.cn/Article/details/gspnzuyqe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gshajkicg.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/gdjysnrpa.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/gpxnberdt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/gspiojini.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/ggpyhnuvp.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gklihqriq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/guhtduhmh.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gdslhrldx.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gnnnwxsiv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gfhpthtkz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/gfowvtrfn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/ggfqvsmvc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/gyozhwzvd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.hesvh.cn/Article/details/gjpdjwgbw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/ghoashnzf.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/gafaopeoy.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/geergmbbj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.hesvh.cn/Article/details/gjtrkylvd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/gnvypfkqq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/givvcpibs.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gjrbwkfyu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.hesvh.cn/Article/details/gemmiuejs.sHtML

Go:   defer f.Close()
来源：http://mobile.hesvh.cn/Article/details/gzchfncgw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gsmegogme.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/ggmzfdnck.sHtML


<!-- 参考信息 -->