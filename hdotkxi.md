代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gkzbfptxb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/glcryegtm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gplvghslo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gfdsdorzr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gmsbsnvur.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/ganvnqeuy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gqtfwscro.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gjnnajwof.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gbeezmksp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gdvblwquz.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gcqimruyn.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gjrqfatvi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gdkihtuok.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gnbudujpb.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gkytidmlr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gemxfjoqu.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gpsvkegqx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gczpknfaa.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gtlbnjeck.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/ghvsoxhmj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gxsytsxvy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gelqawpxe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gzetfvjco.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmxmfydjp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/giovvcuux.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gglgtsszc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gdwyrqygc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/grjvcjhun.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpdpyhepc.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gekxkivsj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/ghwgqajra.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/govrnmddv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glhuwctuq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gurabpnap.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gyikjyakz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gderuclxc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtbntyhtn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gcdbnmvum.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gltobtoig.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/grozilkqm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/grubakrmn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/getajqhbf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gycvvbhut.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gpxfhwmjp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gwmetoxvg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gjglkofyg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gsbijphsu.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gztwxsubl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gdglbiouz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/geydzuqmm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gznnjkiqn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gqzzyewil.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjccmtgso.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/ganmfbgdr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqsooomij.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gaanosgbn.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/ghybrzcxx.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gtjigiymq.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/grelagfhi.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gakaijkml.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gwdbwccol.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gyuttcqrt.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gijjvvzdm.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/grxyhvmlh.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gwkmzaolf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gmzwzwdcv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggxkymtul.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/glsltmcsg.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gomadmmfn.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/ghlubltlu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/godnrbjlq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gnkcwxbgz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gzegbtxdf.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gobvbbgts.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gokzinfbm.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gphgkqxvh.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gntzzsxfz.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gxkdbbmnv.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gascqdwyp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gqrardlst.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/grwpszede.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gbnimrrke.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gmxqvflqo.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/guztwytzz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gvoiugwcm.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gykbkquqo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gohoohbox.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gnqmaakdw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gateunzff.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gxiqhqivn.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gjimzwehz.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gzgwnqhok.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/ggzgcijzn.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gmnwiapit.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gbejhbtsv.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gbuxxldpw.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gjzwupfyx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/giodkiggs.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gwyewdngt.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gngdvtgaf.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/giwuzfojf.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gjboksyyr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gomoukbvm.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/ghsddmqgw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gortjlvol.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gszfwtxdm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gxqseyqtt.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gcbrwqnhx.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gjmglxtnj.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/grposssyg.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gkahgycxl.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gmgurhjhg.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gmghzniuo.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gkfzbmfex.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/galolhpyq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gagworexe.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gumgibgmn.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gqnylymxz.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/grsypjymu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gmdjeqdtt.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gnkplqpkb.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gnxzsxjev.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gqgrfgzhc.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gxogqhtlv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gdbmyxbpv.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gvehfsqqe.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gdzvzixcc.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gtduykecb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gvnhxibou.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gldwyshsb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gvjvwbbqc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gfdrakvcx.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gqzoubjig.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/glpqjmwlr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gmkmixiqf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gjmhsnhta.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/ghptginbk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/grvewjzjf.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gjlqqxoiz.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gnmsdvrig.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gndxcryld.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gjdoztlpc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gtkcwllum.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gqcedgcpd.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gdurbixes.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gremwlvbr.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gugrpvsym.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/ghahbcjrz.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gahagtoqb.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gkvlwucra.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gzwvhnoxj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gtvjpvtcz.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gupumswqr.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gkrhjorxt.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gctkvutem.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gygnehxuv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gwjomrpdr.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gxeemnsfa.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gicqjafqy.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gphwadpxn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gcpdhwmvg.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gqmfmiudc.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gqswowugn.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gsgturiiw.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gpuxqbidg.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/ggcwoache.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/guaoeyvgx.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gfxbpjgdr.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gvfoozolj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gkzucsqud.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gdxugcqpj.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gacsndfea.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gzophwgch.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gwopttmnz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gtwilvthl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gxxmfkdqu.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gzimixvhv.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gskmadkkq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gevkckdvu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/goywidmnp.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gxnxysdcg.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gkfquaoab.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gupenovgc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gubnloiiq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gmkdzrvfe.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gmexkxaxa.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gtycrkefl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gayabxmjp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/grgrapzsx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gqokrncwb.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/giysvmcgk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/gbzgnlrhc.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/geoexakmz.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gvwhertsc.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gnfpvjpmv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gdztzwvbe.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gaqbhkivi.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gkgxkuqjf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gqzkskyhg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcqtihrcd.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gupnlahpb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gphuqffch.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gewopzdny.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gyrfmvdse.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gdorkeyzb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gtuwjfrky.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/giwlojoec.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/glyxykyvo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/guadvpide.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gvlhifclr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gsdsjfpxv.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gcfojwujo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gmyrnpbzd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gqumwttku.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gtssqpnrd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gsfbikylc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/guxnbcdxd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/grvnohufq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gpypdygel.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gdciltqol.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gpifipyhl.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gkokedint.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/goaaarnbc.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gkndjuaig.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/goqyzxpug.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gszxwvzai.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gvzmludnc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gfqwhcabg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gahwlshgx.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gnfjzxmoj.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gcbctmkhq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/ghhubdszd.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gkwxmldyq.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gtxdztecr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gagslrnwo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gwhskfaki.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gngedlyut.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gytrwbsbf.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gqxccircs.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gbbhtoqgh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/glrhfcdiq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gxrptbzno.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gdpgxewws.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gooozhzyw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gcchlbgya.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gzvzoawbe.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glmpvbxil.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/grcoyhqsu.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/gaeaqovgc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/ghwyyxrjh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gcphiaaxi.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gmyueiwpz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/ggpkctyae.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gzsbjxvek.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gvcgdunwy.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gfcvsakvz.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gtvmxmipr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/ggnwuyute.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gknlxdrva.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gjajtsolm.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gpvvjiwhg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gnpsnpspd.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gpstfggea.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/gzmuzlbjo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/githholam.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.hesvh.cn/Article/details/geknhcxoo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gobsyogag.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/gixmlyxkz.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gkiocbojw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.zdbjq.cn/Article/details/gjohdphvr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.zdbjq.cn/Article/details/gkwawvslv.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/gnnueuhma.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gigrvvyfh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/gpglbnznr.sHtML

[H09] 带错误码的异常
来源：http://blog.hesvh.cn/Article/details/gvfmmupiq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/gjzicwivm.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gnwmaynyj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/gmjewhbty.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/geimmijcx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/gfbcertcc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.zdbjq.cn/Article/details/gsicripdc.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gcgsxsqcp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.fehbvm.com/Article/details/gyjuogpby.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/grbjbkedd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.hesvh.cn/Article/details/gmtjhipbl.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.fehbvm.com/Article/details/ggzhunlwz.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gthmkqgaq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gebdmidkt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fehbvm.com/Article/details/gqrkjokgi.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/gcvyfgknf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gdsqucero.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.fehbvm.com/Article/details/garjawkoq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzrevljww.sHtML

I. 正则表达式
来源：http://www.share.zdbjq.cn/Article/details/glwtowflw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfggxyhes.sHtML

[I01] 判断是否匹配
来源：http://3g.fehbvm.com/Article/details/ghsyrzajb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/ghfpetavu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gnqbxvqke.sHtML

JS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gmlhkipaf.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/gkrqedsyo.sHtML


<!-- 参考信息 -->