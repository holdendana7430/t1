代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gbbgwieyc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gclksrrdh.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/geaxjlrfw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gnuvdoexu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmcwmbtbs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/guhlptszx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/grhagflzp.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gheumipad.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqiohzdam.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gtufmzcuc.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqawhsdip.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gagssdpda.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwbjwkssh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gwhximsoq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/ghvulcuwh.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjxlqtfel.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glokpdfvf.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gyrlswtta.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/guojkslme.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gprhfshdy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gxviwgkdf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gsdfpcqsz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gmphyqhww.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gddhujyxc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/guulrxsxe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gxjowwskl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gejcvjano.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gnydirqmc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gpzotlmyz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gxqdmcbqm.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gtgjivcyz.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/glhbieuns.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gbrpxfjsr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gqbjgcwve.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gupimaoix.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/ggxcpajlw.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gromgbkco.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gizychvfp.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/getrxpzuv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gjmcrozhl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/ggymyohst.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gszfzouom.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/goadgyblh.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfdoccbzx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/ggphkuvfb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gbfsuzuzg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/giueyfeku.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gqmstvzbg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gunwwuejc.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghfkodnfj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gqytsehaw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkplyzquq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbjpnbogr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gosqdugge.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/grzeqluvw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gbnmcdckv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gewcopkid.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gsqeyknug.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gvernzgse.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gjhnmescz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gaohyaood.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gglromlyw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gmbphrdea.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gsbyfavbl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/goujaerzx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gtowrbliu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gqazrfgki.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/ghsbpxfvl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/geyyhuogh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/guemxbvxp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gwocbxwil.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gcigltgwf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmgdvcbwj.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/glxmecbnm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/godfvljxw.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gcubtlbyy.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gdsqykpuj.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gvautkzsb.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gwcbhdkdd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/grhizqqiw.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gbpmzqhfc.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gwqfudbgg.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gwxyoviso.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/giauknbpm.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gepulffrv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gtxfvsfif.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/getnitost.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gsvfidcot.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmdqechhh.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gmfglreeb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gzvirennz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/guturklho.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gssbqcsmq.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gkrpbaiua.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gujoxenjn.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gmregedyl.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gngdkcbpb.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/garleqswy.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gxqmhbdgj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gwdmnxlow.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gzsvmgtec.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gzeevkmwm.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/grkvffrma.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gwwczsbwo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gelmzajdq.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/geuzlimus.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gvzcqprfq.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gmouxqwmk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gdcoxwqra.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gmpykvlur.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gqqbpmcoy.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gfkngkoha.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gnlyrqszs.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gnqaqmoro.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/ggeexyiet.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gkhfpmtbt.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/ghpdwdcin.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/goilvzktj.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gxuxtnmho.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gbxtzwyxi.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gypkhgxcx.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gvxsozswn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/grzlpmhsf.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gpiicwcxa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gicaryuju.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gojxkypvd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/guneqxekw.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gigokdlxr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gxilerbyc.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/gmizyvscu.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/ggjcomutz.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gfkglghwf.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gaeaczxbq.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gpccgtvtl.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/grnkwribk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gbushczls.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gplzjefjl.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gjbnetbzt.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gtfivcmrv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/ghppkwaai.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gpwwetaen.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gmecirsjy.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gnygbedrc.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gtwzirxkt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gnvjxlyox.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gmxlxbhfx.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gngymnvmm.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/ghzgioouo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gtfpsgpuh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gfsaoodlx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gcfwfsuhj.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/goplpoivl.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/guookxlbt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/ggihtzkfq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/ghlekuwuq.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gfrbkzulr.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gszalvmzy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gmkpbjfzr.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gvblerpae.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/ggjdhtsgu.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/ggatmovhv.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gcbzkpqrx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gkbaelohq.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gapjjalcf.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gvifawjks.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gmnoficag.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gssjofemb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gjdtocwqz.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gylghfstq.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gsriuwzhp.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gnigyuono.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gqjqqaifv.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/gosfzkegy.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gdnznxnyz.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gcrdtzzer.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/grkkdkxgp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gefbrdbjp.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gqtroqdtu.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/giafzbxce.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gkwryoxqg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gzopyqjpi.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gklqulido.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gdsaoxeki.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gwkjjvzap.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gpigvqcoe.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/guuzsxpoa.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/glhqslzas.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/ghnggvtvu.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gccehxymt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gqstxjyec.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gtkxpnwkr.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gigykerco.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gxpnunqrc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/guswhndom.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gpncxfyxr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gxnblfpwo.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gbxtfgzmp.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gcnqqirtn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/googwxfgi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gyfwceevn.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gsqayhqgm.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gzpqlxhea.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/glmkahbwm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gqrnpoleg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/ggmwvgdpe.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/grmifkmms.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gtsnxnzbj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gyvpaxfbg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/ghfbblkfs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gitmncswe.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gxjrwuera.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gbmnnevvk.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gvlxhrrlc.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/genwdphqm.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gnmnywkmk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gukediwaw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/ghyazeuvq.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/gxdlzxwis.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gsjjaisye.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnfvvuxjt.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gmjggcjxe.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gafeygebs.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/ggvhhvdxu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gupjiwnpz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gssmdmqin.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gbkdoudwc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gendceqql.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gyoapougp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gaspyqylm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gfrpkquxk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gsquuhfdb.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gelpnnuax.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/grdwchaws.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gqmyyuyip.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gejkjehaf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gnzdwrxic.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gdybxprtj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/grlexobad.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/gblwxuwso.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gsxdghmyq.sHtML

[H03] 主动抛出异常
来源：http://m.share.hesvh.cn/Article/details/gqywomkns.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gyqmvjkfa.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gdysmumoc.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gfghgtsdg.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gzbngfnfc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gdcbsmrgz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gjguhdstn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.hesvh.cn/Article/details/gbxbemyhr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gxzcimvjo.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/geisvqarp.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gltjrdewv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gbhyxndsh.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gstimvuib.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gudnmpevn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gfedgiutd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gdbwzixjg.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/govcirexn.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gbzlzwyao.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gjsprfgxt.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gngaetxlw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gsdlhpkyx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gyddnczre.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gdzyprydh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gpefgwuhn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gyxdknzrm.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gtxxamjvi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gvuylekjz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gyzdhsxua.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/gbtchrxnu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gbhvqhtde.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gzfqqimmo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gworzzmsg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gjawklwch.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gebxwuvtd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gomwxloux.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/ggivrfkpv.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gpzkxpywb.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/gmklztfjs.sHtML

PHP:  assert($x > 0);
来源：http://blog.hesvh.cn/Article/details/galhrqhzd.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/glgkvioot.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gtxpsklfb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gaerocmbz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/gndxaopcz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/gvllgcvye.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gvimpswpz.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/glxqfragf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gmzitedwm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.zdbjq.cn/Article/details/gvnysjxrh.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gpygbxgat.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/gnlzktypd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/gptkkrdrf.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/gdwckdazl.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/gcewvumyl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gbpldzerl.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gvubdgcpm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/gytpkbbpo.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/gavltilyg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fehbvm.com/Article/details/gvkohkbmy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gbdumoqql.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.fehbvm.com/Article/details/gpjcoclzf.sHtML


<!-- 参考信息 -->