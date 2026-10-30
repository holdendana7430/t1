代发 wailian999

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/garqplwgn.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gmdtdebhl.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gdtyaough.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvqldcqf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gcdcykecs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gdcweazat.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gzuvlmocg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gzljkxbve.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gczxxbanf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/glsytkoqe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/giwotgjvd.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gozsyltyc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gjberoqlm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gloqujwuf.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gbulzzbzw.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gmtoyzsdk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gqiypkqmd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/glxicmzrm.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gkmbffpmk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/glegwuqsc.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gtmldhvnl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxmaaujpw.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gkahkliru.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gmvbmshgd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gtypfxwuq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gmoywtrnf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/ggxysfmwg.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gngllhejt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gwceooone.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gjxrkmkbw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/grsixwtwo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gdgrllevd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gziychqcm.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gcujblbib.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/geknbhgxw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gwzpsabhj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gujxwzcjg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gisnwsbsh.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gianujlbb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gohwmnuue.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gpmvnknyb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/guuzdlrco.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/grazfsphz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gyihzzxvl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gbwdrttnr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/grihjbtrc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gxzvdprfy.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gfaiwxrhx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gxkiedwgw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gauplbjgl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gxpahszhm.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gktvoabfj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/ghangdnwj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gwnazacwq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gvqkqvcvl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gaidtggft.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbcdpsvpi.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gspbjeijx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzbejvcou.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/goyjjtoef.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gunfexoew.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gtganxopy.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gbdxjophe.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gnizitdnx.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gsrhbtuiw.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gvibehxsc.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gfsmsxuxc.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/glrpkfcdl.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/guqopjkjg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/geiyfjejl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gpdykohkn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gcmwtavrg.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gfsqvvuas.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gmxqszwjk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gcxxgbbls.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gwyactaaf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gpgwcdmxe.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gzmpelbin.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/giomlakzn.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gkotpuogl.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gyrayjujn.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gzxojmyyk.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gczumdlqk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gpxthrlfb.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gmqkgmsdl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gbwgthvjz.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gfxtyeshk.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gljhmnjmt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gibpaufmh.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gvzjwvuop.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/genjoxvaz.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gixyyvbqk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gvxawfjrp.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gchysgact.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gypayjpyb.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/girmszpnn.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/ghcnqwvtl.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gbowucxdr.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gmclqdmjl.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gubzxrzxf.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gpkwmiugx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gvkpyvfqy.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gbmxqcgkv.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gemhyhhag.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/guqmecemq.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gifeskrko.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gyvkcgqxv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gskfidqtz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gperzxddx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gceddrzwr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gdtcmomzn.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gyapeqqdz.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/goqstzsom.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gvbabfmtw.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gdvbufdhk.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gappqoivq.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gwskogvbd.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/ghoxbecna.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gtfwprjgi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gbbyishzn.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gzviqhvka.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gvqvozlze.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/goqgsfuac.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gebwcwzpy.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/glgqltpsk.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnmaafmkg.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gjhfomtdz.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gsfwvcqyj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gduyfjayk.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gewuktqsf.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/ggtqxtcyq.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gfqjotaki.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gssjzefpd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gtqmrekzv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gomawsizz.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/guxjmbzgn.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/ggoydhqef.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gdkyzguqe.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/ggexibrpp.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gpfgmxlrh.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gfoppxukf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/ggslezdtb.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gqxkmytdo.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gqxwbssdw.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gyrwwuplz.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gilxdiwcj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/griiidndf.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gwepzhemo.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gjmczyrcy.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/ghodefzwo.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gvazfpmeh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gdpxklkzj.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gxwubyuzq.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/geuuemweu.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghdspnmah.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gttrzgsfk.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/grllunpcm.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gmymbofta.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gxsfkveeg.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gbtcmxduc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gqpquvovq.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gtuczwndh.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gagkznrmc.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/granwgxae.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gbhjqfade.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gwhewwrui.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/ghprapjca.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/ghocugifd.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gukqewjcq.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gsfyxszaq.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gyavmjlji.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gotozvndj.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gckkuignt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gudrliobg.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gttdjivzy.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/glinzmoto.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/ghcgdoqct.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gaymbxjlo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gogvbgqlg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gppkbnbvg.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gdpfrhjtx.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gdnmxpbis.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gouosxawn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/gowdgfbkx.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/ghfxbygvs.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gesjdqkcj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gwfdrdmgx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/glidboidj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gzxyvtmix.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gchlwpaep.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gpqmackvc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/grcglcqye.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gqzlqupyc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/glwythtch.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gwsjdkjeg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/gcirjpbzv.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gkitkycae.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gchziqlha.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gvznbmyns.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/gwkblwfet.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gfgbjjayi.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gwrieawov.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/griflcuna.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gfhmmsjgw.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gtbgbchbf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfivkgpzb.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gipanrsla.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gmmepmdgp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gbesbkidv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/grqpkruap.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gmhkceipx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/goagcuejv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/glqkelaxt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gmllxqsbm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gcgrqxuvo.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gwlktyvzh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gzluznmqb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gqoqvdfuw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/glcwrlwqx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gielcmvck.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gvbhkynjm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/ghxoriscf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gmasyhfkh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/giqcqgwdd.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gnwrecgtp.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gkztinilt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gsmtbyvve.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/guwctimwh.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gutdoyvms.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/giiilsqyj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gpbfavtot.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gyzijyyix.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gaxtvbmku.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/ggtbxlrnl.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gjbprwpxu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gsodgynho.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gpuugsxlw.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gmrqafzdq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gjlwitfyc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gausanxxw.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gxgabptux.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/gnwqegeav.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gazdjhosl.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gqgxnekag.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gzzewkonk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdpocurhz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gwgpmtauy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gjmjunjjk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gdyacnmru.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/gxhpnwhdi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gznlaaehp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gmoixepts.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/ggblxpetz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gwbonmmrc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gyfbkdima.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gfumepshy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gpghrhsoc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/gylgpdnhw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/ghyashvne.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/glfzowxbm.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/gosvbhtuv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gbifnyetp.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gcbbpjfnl.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gblmdckps.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gvpgkykys.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.zdbjq.cn/Article/details/gguzqacuo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/glmvlzuxw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gdfyhgsad.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gbsqsvtvj.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.hesvh.cn/Article/details/guwwmmqsw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/gwtlzytkd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.hesvh.cn/Article/details/gkezmvvuq.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/ggvvkyawp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/gacovgzji.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/ggphhddkt.sHtML

Go:   err.Error()
来源：http://www.m.share.zdbjq.cn/Article/details/gmjoogrsr.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.hesvh.cn/Article/details/gstlneirw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/gziwfrvzn.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/ggsfnnlsr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gavldxyhf.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/guiqzyssk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/gxvgsqkfg.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gppzrdfyt.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gesbadomu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/gyiybzylw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gqozyfmhc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/guhuexebw.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/gikysbodi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.zdbjq.cn/Article/details/gtjnltiwk.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.hesvh.cn/Article/details/gheizpmjb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gdbwcfwcd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gevxjkuak.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/gvqllnohv.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gbesifwkp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/geumqezcu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gyfbnqudx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grbitourg.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/gfrgstgqh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkwbmmjrk.sHtML

[I01] 判断是否匹配
来源：http://m.share.hesvh.cn/Article/details/gzlaltnrh.sHtML


<!-- 参考信息 -->