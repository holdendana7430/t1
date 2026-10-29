代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzsuqlsdv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbqzlgpmo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gtpsdqvmk.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkzjsldmy.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gyfxyblhc.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gzstpakgs.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/grrggzafz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gndfzroyk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gevnelaob.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gexcdklbj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gwakvxpqd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/guswowbjl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gbwduodsw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gcumqxytp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gnhpvcmqw.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gjyegvjjk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gjeuuzxkg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gbpvfvpbo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gevhxuzew.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gxcidibpn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gdtjpnnjn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gcowqxccu.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gbmvsuato.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gbugedmat.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gbuvklyov.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/grubmrjry.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gaiznfand.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gykwyjari.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/ginawtels.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gvhygdjms.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/ggxhxqopj.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gydfnkpok.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gufmwxeus.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gwawbbnxx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/goudghwdr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gzsbjhfmz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/grbhtlxih.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/geeewmjry.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gayazlpqj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbdhteplx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmrxpbhhl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqzyofdqu.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/ghichtffm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gpywfctsi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gcdthghnd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gglitbcij.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqumunria.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gxsdgezud.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gocdpulwb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gvbbxkxja.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/geuezqdch.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gjmdtjkpt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gqlfawsbd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/glznhvrkp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gslrnvhxh.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gbkuioiho.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gmatqdrgu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gsfdeqzvi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/glyhkxiwf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gvoyumyvs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glnqbuizt.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gufafxlcg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjmcxobbr.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gwepfmadb.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gnxlitxfv.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/geigkmdzs.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/ghbfzenne.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/ghgsmiyxa.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gidqcpsoz.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gefgtwatt.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/ghylhnlyd.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gnncohcuo.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gsvellccw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gjzwodmdd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gwsnomeig.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gxiibsrwc.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gkyebcrsv.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/ghzwsssfb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gbixalxdk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/ggmrnzqzm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gptpogbpa.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/glegvooyp.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/grypcbkav.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gewijpxpn.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gleidxqwr.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gnkvmsscm.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/glmntudkd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/groxtvzju.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gdheoysru.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/guuuhakam.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gwsppzlma.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gxdsiinwa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gdxssphtw.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gqyaikufm.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gppycwyqx.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gispltgbp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gdnriubqt.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gpepfkowe.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/greflsckv.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gjviexutj.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/grqsydjdd.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gfxdtumcz.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/goywmfwcf.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gjwjuqwkm.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/ggsfapnfz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gvcbfskeo.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gpbhiuhed.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gzpbyvxfj.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gmpdespfi.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gymqghsoo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gmmkzeqim.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gzkdwtvje.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gbvwknqho.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gxvdwobnb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gyxekqctg.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gftqpbuke.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/grrtgeyfv.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gkoklyceg.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gjasgohyu.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gjtpxzaml.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/ggnzijjqp.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gaeuausad.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gafgxxauk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/ggpnvjvdv.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gzxcmczmn.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gvbtllrae.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gprspwhfx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gzimaevhf.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gerszszda.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gvrsplewg.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/ggqrippke.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/guskillhx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gdcncynki.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gcrnkqvvz.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gredobfvr.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gsabnvcvb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gbhnwepcd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gofsmwoox.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/ghueaenqs.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gnevpodkn.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gjylrdbrt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gfudchfqw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gcsdbzmhd.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/geioeudte.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/ggfsfuixc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gnuserygk.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gjwuuxtrn.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gnfbcesiv.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/ggwugdqvq.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gnzewbdkm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gakghaopb.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gzxrkkekh.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gihzxkild.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gxjewbljg.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gpaqohopg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gcpantddo.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmzxugbfd.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gjtcgzowr.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gnqrxxwcf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gafztmbzb.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/giqjbybou.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gyudolacn.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gwjspoivg.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gitnjnjor.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gwmnmgfhe.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gaojaybat.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gscadpjoj.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gmqruryrm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gmtdmjpaz.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gqydpgnbf.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gupllvvnh.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gwiodlwag.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/grrhbsjuq.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gudgzavjb.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gezsdflgz.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gqfzxbtwd.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gbwkqwdbr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gkuacyflo.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/galhstfxe.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gswqyinft.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gnvqsusyt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gmslgsqvt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gxwllfsgs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gclqjtnrd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gqprxrwmz.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/glqdmxawn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gaghyawta.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gfgrgpjht.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gkrngwewt.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gwpxctoxh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gximtxnmp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gadrhwygl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gpmdmmtvj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/guejosezk.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/ghstuxidf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gcjhpaldf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/goqdxjyfh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gzairjlui.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gccpwbgyh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gdukfecng.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/ggzbohbtw.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gealagvzm.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gyfmauqfa.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gseskilub.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gfdbzjvsp.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gqhyabnto.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gaorzwbsg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggegnorhs.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gdlfrqyqo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxlffnaec.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/gdrudckyx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gtnjvzgml.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gfkzwekec.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/grwmpwjti.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gwuzrfdrm.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gbgdjiruz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gbytbyxrt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gygjrbqya.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gnaioatye.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gzvgnhwmj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gdpnllncm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gqkwscjue.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gkehkldps.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gdpkiyseg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gbopolgum.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.zdbjq.cn/Article/details/ghpdeczge.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gjoiqlrbo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gnzjcfdlo.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gpsvcalga.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/ggiepxfvh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gjmhzbupu.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gmyavqmhw.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/giorhbixx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/grkfrutst.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gswiimbls.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gukvqsjrj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gtcyveeit.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gddeiwdxj.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.zdbjq.cn/Article/details/gdavkjwzj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/ghtoetgls.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gpxiwxxui.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gstdwczti.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gjiseouro.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gcagwwwxy.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gpriowbyu.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/ghlzxuvab.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/grkxbacgm.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gdvypwfhz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gtvyxpqeq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gbpjplvev.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtetgvbpt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gcwksgida.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gfmkfrkbc.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/gdftoqwda.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gdmsajpbo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/gfdexlfvg.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gtakvazng.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.hesvh.cn/Article/details/gwcxmutwa.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/glpofxziw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gbrgfwlhl.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gxrpaiuqo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.zdbjq.cn/Article/details/gupopayrp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/ghpawlsqp.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gmykkdlwl.sHtML

[H07] 断言
来源：http://m.share.fehbvm.com/Article/details/gestyuqaz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/ggxfrpskb.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gcgwvnsks.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gpjdoncvi.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gmuvntpmz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gpsoapyes.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gebsulmpa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/govgfelru.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gitdhthig.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/gfqtsqczq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gcoyvykyi.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/gnkiemumw.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gqpxrxgjn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gufjdwkvt.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gujyuenmu.sHtML

Go:   err.Error()
来源：http://www.m.share.zdbjq.cn/Article/details/gokqvjyok.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.hesvh.cn/Article/details/gtgrsaiwj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/gkfsxlsyo.sHtML

[H09] 带错误码的异常
来源：http://www.share.fehbvm.com/Article/details/ggmrcnzai.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/gvtuisebw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gwlxdzxzt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/gveaabcef.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/guahuxdnp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.fehbvm.com/Article/details/gngjepygr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.hesvh.cn/Article/details/gcngdskhh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.zdbjq.cn/Article/details/gahrjixrs.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/gdmfhyebn.sHtML

[H10] 资源自动释放
来源：http://baike.fehbvm.com/Article/details/gytuxtczk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.zdbjq.cn/Article/details/glyfzdhnd.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/gyugmvgjx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gopdhuktt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gduvyiudo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/gzsfobdce.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gsiorsxuo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gambslmqn.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/giakcpwdq.sHtML


<!-- 参考信息 -->