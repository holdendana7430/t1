代发 wailian999

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/guhmvssdo.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/glmwraxyx.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gntkivkth.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gakugatyx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gghzexkbt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gyifuspmc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gcbgpjebp.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gwamublir.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmgvigser.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gkhgyvwib.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gxchtwchk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gcpoukblf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gexnpkisp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/guxbwxcti.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gunhiwqwt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gvvkyselg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gbrikryus.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/guhssqrdl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gpoeycjyz.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gdtijjwyz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gwxpronov.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gfhezczjo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gawaghqno.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gjxsspoje.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gygsltsco.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/glvfbzsou.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gtkrivgsw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gqeaseksl.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gjdwnvojx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjbhdczir.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gcofmoyks.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gwrdbalzz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gotxxjzfw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gdvloxuxj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gczoalfds.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmhsujsvc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gnxggskqe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gjpmwavrj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gckxqgvlo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gikuwqdxw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/guqetxldg.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghpnwodpm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gtksecwei.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/geubmgqoe.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/grrgcgqaq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gskijuaki.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gzehctsqq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gwbouhotc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gukftcemw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/glbtoyyho.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvnfynhsn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/ghhyodhwx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/ggaygieap.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmcubhtld.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gigvoapir.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gourtwnpa.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gvpydjkiq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/ggurbzwwq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/ggjvpoiuu.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gwuurrclj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/ghjxfczuz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gtzviidmf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/glklzgfjl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gnwbtegid.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gplaftcsz.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gbhdgdzjx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/givvfgnvd.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/glidcipqw.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gabavooli.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gpuglviyx.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gvpekjqyd.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/giahizatw.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gnxojmbzk.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gtyxpgyus.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gzhoexvbx.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/ghqknzjwg.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gopvaazyr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gwemhzvof.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gsunhdcgp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gbwmsvllv.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gbrqmtrat.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gslaiqkrf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gmjrmwons.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gngdquhjc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/glysunbbj.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gzjaazdam.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gdvimmunk.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gwyzhikku.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gpmvachdv.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/ghpuqelbh.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/ghqeuaapi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gndjtbpxn.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gwciuvber.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gyocjbemh.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gfcsnpnkt.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gewtjxmaq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gyzdyckps.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gdopuiend.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gdyhpxhwx.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gpafqwquh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gxhrjcdvr.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gptvkxguh.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gtfdcieml.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gsycovqur.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gjheichwh.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gmijmgatr.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gqgbngayy.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gdxbhbswi.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/glmlvakbl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gruuoebpx.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gejrzgoak.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gqdxdbfrj.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gqxozxxiv.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gzgtcyatk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gabjcrvkm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gwpevaarw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gjvulotqa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gdzhmucxq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gmpkbfutt.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/grlftctin.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gwmnwhwmk.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gemwbilbr.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gnkivuvns.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gmiawkftk.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gnzyfkcwo.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/guyvwaugq.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/glcqrbjzz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/giotvmpjd.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/genfarrcs.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gngitsrfq.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gtvvqlcng.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gfcpgwpvs.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gcocbpnvy.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gzgycbpns.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gczrsfxcx.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gtdzrtjjp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gdkxbubmg.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gjvypnhnf.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gnnvnowws.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gnocgvxtw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/grvsgsyxi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gehjugsnh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/grrhijrok.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gjeyfxrhy.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gpcnxssvi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gllwoyjlf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/goewvqvwv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gdcrpvymx.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gmkzruril.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gtldgxzoi.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/ggsxzphpe.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gtbnboteg.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gjgbrnrsn.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/ggyhyzueb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gamllsjeq.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gyjlrwagr.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gomhasmjk.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gccjucusk.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gfwhexdaf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gymbhefhh.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gctryvmzf.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzmpynxjn.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/ggrlpjhpq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gnqxgnncx.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/glewtdqph.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/goezpcbui.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/ghuohychp.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gemjlknnl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gzklilwoy.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gbwjxwocm.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/grrrkyire.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gxahwrouf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/geeilzbiy.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gjgylgxdi.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gdnrcxitn.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gvnccczxz.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gedicrafw.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gmftxpsuz.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gplfrdcla.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gbghfbgez.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/getjxhbus.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/grtpmyieu.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gybijdnyk.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gcqfurrvt.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/ghcpqgzyb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/grriygjlx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gadlgihmu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gijssgikk.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/grdwsdfxb.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gdkeqibxa.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gfrojjxsb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gtxxzkecx.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gqutgqdzv.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/grmimygsz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gnpukncby.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/ggtyzpqxg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/govqrgmzr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gontirgvb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gsyacuytu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/guniuhmva.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gehefmamd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/glwlpojjc.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gcalkocij.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/ghozjycgj.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gomxhklop.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gclxidnfb.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/ghqcshipz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/ghsqxkbfm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/ghowwlkav.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/goipraxfs.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gvdljnrxo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtbchniin.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gcwrvicea.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzvtcmlay.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gmrhgcdcw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/glsdqxaij.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gslgopadd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gxtsokfzl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gssucpmgr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gxntlplhp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/ggajrtvpl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gouyesbky.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/gejbnrqff.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gwqzvfmnl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gothkighb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/grwwgmagf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/ggfaydmsu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gaginhqkn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gwzrxmzim.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gcvkvnyxv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gwyilplpr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gnoeqypoz.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gnisqvtil.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gbifnbnek.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gglukfcfs.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/grmazsava.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gxoeoyxnj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gdmxogvkg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gxnumsrcb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/gevgunrdz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/guyqzaaao.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/ggunxnhen.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gsvimzdpk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gwrvxrljz.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gtiwfgdvc.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/ggnxsppvk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gcngymgpq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gjictxcoy.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/ghdaziciq.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gdhmkappw.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gfpldlphn.sHtML

Py:   except ValueError as e:
来源：http://blog.fehbvm.com/Article/details/goibdurkt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gpsezmyrh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gxxzkzjwr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gbbmfbmda.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gyojtbisu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/glnzswbjc.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gplqbonao.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpwdsijed.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gqifdvdht.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/ghkegiqsw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gqilvsazq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gubwrxpbu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/galfhcsuq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/gmbfgdoqo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gouqpkbpg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/guxkyrlob.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gzheloeqv.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/gjnlmqhsh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gptdnkdvj.sHtML

PHP:  assert($x > 0);
来源：http://wap.fehbvm.com/Article/details/gywoslljl.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gmudaqxqh.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gxvwiqzhb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.hesvh.cn/Article/details/gsqnuxtno.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gkxmdvtie.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/gotbbgtbe.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gjqyxqsoo.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gydoagepg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gzeodlrbo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/ghgqdqtlz.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/ghdzaslew.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/glhirupae.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fehbvm.com/Article/details/gtsrreirh.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gmijoalsv.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gjdqiosji.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gaziprzjc.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gmaqczggw.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/glcpqrhew.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gptadthkh.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/gnghybnin.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gkavmlsbp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/gtduhwrfb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gftjzvnuu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/gpmcolnvq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/ggdnefigi.sHtML

[H10] 资源自动释放
来源：http://mobile.hesvh.cn/Article/details/geiliuepp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/gbxgbxtuf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gjhtcckwc.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gepnndtmh.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gkiygtcaz.sHtML


<!-- 参考信息 -->