代发 wailian999

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gbokvkrpn.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/glrxldbsa.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyjveiluy.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gqrsovbcj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glgwzlate.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjuugndbq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/geopmqzhk.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjmaojyaf.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnovvkphw.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/guxayphud.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/grsswgbry.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gkkhuswcx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gggfcfkvd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gcbkwvhet.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gsqxbrkwe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gzmmieyak.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gylulccwj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gmlcpufon.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gucsyyglk.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gwrkemfle.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/glbjaskij.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gcaqhpeyu.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gsihedmri.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/ghomujwmu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gdnghadmi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gqaajwngz.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gnknnnztz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gnmvvteoc.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/grrmnqelv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfudwpkkw.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gufwolpgf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gjfwcxezv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gzncjleoj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gdynjnlhl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/geqzplqvl.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdcfexrwb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/guchzsdvj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/grefvigof.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gxcaefmel.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gxwnikwze.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsxfxyrki.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gvdrcdcuh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/ggyytfoor.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gycnxrzrc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gfbumsjue.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gqfeogzoj.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gejiphiau.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/grbzotaim.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gjbwcnudf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gafjknlpa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/grvmhelmu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gmcghqzsw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gvxivmbvh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gwauvuowa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gmbbrxfft.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gggywahoc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gveejukxy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gbsuswrgs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gszspqkyo.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/ghheyhqsu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gbozvknbg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gyqxwhcot.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gkbadyzpo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gjffyamot.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbynoxkns.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gvumpbytw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggffagmpp.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gaetgibck.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gttpvgqzt.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/glfwckgab.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gjaswirsh.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gmzpbmnbu.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gjbfmjnzw.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gcisrznzq.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gyaxukwql.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/ghfewfmqy.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gkvuopdrr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gifbizezz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwkohmlfg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gaogedvnq.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gvsyxmlke.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gsyvujozv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gxdctskdk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/goocronlf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/grrxmzytx.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gzjdzipmc.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gcqlehhgu.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gfqizbmqg.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gqsxpubri.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gsyysdryb.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gisefiiic.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gzikwyogb.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gkriwfkeq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/grmbpyapf.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gjzjndmbp.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gwalyxkyn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/guqpkosbl.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gkowszsyu.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/grqkdgnbc.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfoxkkhrm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gcqioerft.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gjfjyspfz.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gtbszywpt.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gjqfzsrcs.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gtzbzzfsg.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gtgchhvzr.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gzarzxcxu.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gmlfgirzv.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gelisamad.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/glkcahzku.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/ghivoakly.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/girkdkucp.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/goyxiskqh.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gvzqejpru.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gomlawmim.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/ggvqfszwd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gsitzguof.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/glfgkpygc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gtiyhbgyj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gnzsypnsb.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gxzrxyipt.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gsdxxywlu.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gipsrxqka.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/geyjzslvm.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gwmfahame.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gblpykkan.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gofuizpxz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/ghqoruzmb.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gcwbshqvi.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gnzpuyilo.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/ghudtrmht.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gcrfbgfzq.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gtkwtfnzb.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gctjbuytg.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gkbrfbnzy.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/geovgglbb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gggmgrmzn.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gdjpswrwa.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gmonvvuvd.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gxndqhrdz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gebsghmcy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gokdjyyyw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gqhnhqocs.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gfljvyzko.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/ghthuezkb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gtyxskxso.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gxltzhwxm.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/goycfdsny.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gewublttt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gxefoyixi.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gmbqhnxjw.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gwbyhhzha.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gurbchijf.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/guuywmila.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gmtkuikmm.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gkwvlkkyq.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/ganufvzzj.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gdjsthldo.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gwzrfdviu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghxruzkjl.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzydvgdgt.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gdngydivv.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/giksamaky.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gqosqstky.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gcookrtho.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjzligkzv.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gjmrvbnmm.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/ghwdnudfy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gcvdwygmq.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/grnqfmiim.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gwwisqzxx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gqyvoeodw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/ghakkklja.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gkyjejalc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gpxxdagbm.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/ghgdbsikf.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gmtqvacbb.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gngzuwayz.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gztggdmgz.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/ggtcndpam.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gtezgqsad.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gkxrlkcta.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/glsaopzkp.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/glxipwdgu.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gfselgvrw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/gesjguihd.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/ggirnxdmn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/guutkhyan.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gswnbajxz.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/ggtfwdpuv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/goodqveap.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gjoiamjtg.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gowhkzveo.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/grzojisjn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/gmggucaxj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaekyryxh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gcamrduwn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gkgqovzmh.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/glxoxvwjm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gmirrbhfs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gultkxghs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gvgzjvymd.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gdtjycknd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/gkwmcwabe.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/glsmnyfsn.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/glxgogska.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gqrhpuhas.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gmrywxove.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gzvexwicz.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gbnrelcoa.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/ggpezwsns.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbwudcwuv.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gfsemkpwa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyvfggcan.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gfaigjaqd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gnmjorimt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/getkvbxea.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gdpeywgtn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbtlqtqjk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gbwgpokqc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/ghrgfjcca.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gfcrurvwo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/gcjlpwoob.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/ggylqaigi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gnmdoejhd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gsrhlixrm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grddujjfq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gaiiarqvj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gzrcxzucv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gycztyxvu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gfrnxjlia.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/ghwrizabt.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gzfwbmpat.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gqtkchsux.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gxgcqanpy.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gdgotlwud.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gytxqzhni.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gfjvwrcmu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gzmuvzocw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gtxtoeoff.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gvztvolqw.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gwgedxypg.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gmhxyuylz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gwvsxlpub.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gmqdpqdgp.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/ggbcksfgm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gocodzgpy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gipdfdjbt.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/golarwybi.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/gwhbguamt.sHtML

[H05] 捕获特定类型
来源：http://wap.hesvh.cn/Article/details/gpbzdkofy.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gjutzgmcd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gjrrvfxxu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gbbrokyjr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gyoncfajp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/guaijwgnh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gfwjopmfs.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gytaxfupc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gghxwhuqg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gzlswmaox.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/ghwfaiclo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/grpbprxkg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gxjobncjt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/grzedatvc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/gsgcvomae.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gusaiacpc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gygrnwspo.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gzakeprfo.sHtML

[H07] 断言
来源：http://www.m.share.zdbjq.cn/Article/details/gfqvmhljg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gkyanueup.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gfiplafwo.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gjswdquog.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gxxepntmi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gwmkjdgku.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gvwhoclyb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/ghkxvzlwr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gpyxjruqb.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gyzmtkslq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gzmqdmtpe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gwmdoqdzj.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/grwcerjhb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/ghuqeclgu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/ghwhnuwqb.sHtML

Go:   err.Error()
来源：http://3g.fehbvm.com/Article/details/gppmefzkv.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/gumifporl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/ggkvobkhc.sHtML

[H09] 带错误码的异常
来源：http://m.share.fehbvm.com/Article/details/gxdnfplni.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/glifjflrs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gprpidjfp.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gicksljxw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.fehbvm.com/Article/details/gvgnmwuaf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gmdkgsxts.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gwgoegmtn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gkpdpppgu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/gegrfmjvk.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gemyvubvc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.hesvh.cn/Article/details/gsxyoaivm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.zdbjq.cn/Article/details/gtdnelwso.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gptxsrbpy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gehbisare.sHtML


<!-- 参考信息 -->