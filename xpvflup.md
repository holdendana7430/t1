代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gaorlhhnp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gumbxxiyb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/ghlfrzicy.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtitgatlx.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/giwyoovfx.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gumavygwg.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gczwvwgad.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gbyvevlga.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gvksljnim.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gmczdooyl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gcrlqtawv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gvjlbnflj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gsrrxuixo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gqgufjlyy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gwqdvvjii.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gnoqkarpq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gcxxfsjjw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gutpqlbwr.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gcujefypa.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gyxfphrbj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gjmtjauvx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gssgcgpwz.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gmfzxhbbl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gijnbgyoc.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/giwepfrfv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtlvgslfl.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gcypnhsjq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gxozwcrzs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gqkuytbqy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/glbctubej.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/ggdghsgzb.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gckaszecd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/ggjlyrznq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gequabmeg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdklwsggk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/giihlnnuy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gzivtcypy.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gvjtdgvnn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gbbbkfqxu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gfsaxeicx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnyfvaxae.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtpyvhrhc.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/ggxxbjylt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/guwovtbke.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gwjddqdpr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/ggdavokfe.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpltxfodf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gjlhebakf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gktcyqhbm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbgwctjhh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gyummswpq.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/ghurjmuiv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gfhuaxojb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/ghbskjlwg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gulusuzev.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gycmdrnyr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gusbswely.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gogyclkli.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gxxccnace.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gclnqlqyu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqatkwdmf.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/ghhzkljge.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxqsodrhs.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/ghxzmyqdh.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/ggqbfwthb.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gzcpqjosn.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/ginunsgnx.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/guzkmfpph.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/ghqfsfnjy.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/ggsetrvyc.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gflrqrhhs.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gtbbvqicf.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gzjxxpwdk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gosiashod.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpnnbrqlp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/guktvgcky.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gdgclptkf.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/giwrqnylr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gosbpnelt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gikrjmsne.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/glzdwzjbi.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gbxcjepwf.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gseomthxv.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gizczxzla.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gzqdscnci.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gmbizygwe.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gbpsgzmep.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gkckdhmcf.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/goxvqqoia.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/goigvpmgx.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gfnapodjs.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gpujdebel.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvzxlspnk.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gnudjgdbr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gyusnpwyp.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gxpzovjda.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gptegvmng.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gmdzthoqc.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/ghjdngcqi.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gxddqebos.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/glnlhokfl.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/glayircqk.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gvwxzlbci.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gpbrcjoow.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxniimykn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/glyetkvqd.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gjjjcdyxn.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gojblpukn.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gescgtnao.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gceciufye.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gbjfnsljt.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/glcrhmfph.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gfkbufqro.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/grmvcphzh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/guaxoclpk.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gsenuldno.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gpgamibcw.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gzdmrogml.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gizztltyh.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/glywctwyo.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gbopnrjah.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gwyyactcb.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gqjssndkz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gyvvfwtuw.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gejbksjyn.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gcxjcbqtx.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gwrofztsx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gpzzouejc.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gkyjesthr.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gfypvnjob.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gsacqsxtp.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gpnkkoauy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gmoujpgoj.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gbbvaqbac.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gafwwzoox.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gmhvcrqvu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gqfklwwwz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/glyztmsux.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/grhotnard.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gzclfadff.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gasdydayr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/grlfbfjau.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gqjsatwep.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gokhgpmyo.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gmcjwbtug.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gvnrfzmpf.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gekqvnify.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gawiiavfl.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gzoqvzxky.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gwngiboyp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gsncsktzv.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gzysqjtlm.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gwmxrzfas.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gndnbiceh.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gcpmqkhsi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gluhoiacm.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gxaqyzitw.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gwibaontr.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gacqsidxj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/ghvoqpffd.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gqrkccran.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gsmlvojeb.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gmrbgozcd.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gpwckouss.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gltdkcqnj.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gsdjzbovh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gxzvqtgbh.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/goukacuws.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gpvmasufi.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gcrglqwpp.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gsjsjadah.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gmkxaaqdx.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gykbhldyv.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/ggoiwbwfu.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/giyyywhna.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gwnerlcga.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/ghqdodpmy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gwaxjgqll.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gomhvrinh.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gnjxoanbr.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/ghwcvppux.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gtqpwbavm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gcimbofsq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/gzdlogtml.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gfctthzby.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gkkjltfel.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/gdagxxjmq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/gvfxttbsk.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gbdfqscek.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gmmgommsi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gkdukuznl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/glwogahxf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gsvtlfkxp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/goibsacue.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/ggdtsrzur.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gtblqklnr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gasjkyazi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gsjdayzus.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.hesvh.cn/Article/details/gbgfyhkyc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gornierjg.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/geqyuhevy.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gwffogbxx.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gjteybwku.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gjnjguwaf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/grgkpnibu.sHtML

Ruby: obj.instance_variables
来源：http://baike.fehbvm.com/Article/details/gpgdjgbdk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gudmsetnx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtmitfntb.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gkrnzvxbe.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/giybhrwjx.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/ggmgkeuqh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gvrxencdy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gjfzrszep.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gywbuhhnr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/goxxxtwez.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/givmgndfm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gbdgaqykt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gaaixofxs.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gordnuifk.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/genudgzoq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/glphxrvfg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gvyjdeemm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gogjywymm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/ggzazferv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnyyqqnfr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gldpakfpb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/ghmhbeluf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gotvqblpz.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gyeiadolq.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gcwhjmjxj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gajmqzjlr.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gjxwvuqse.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gkmandoto.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gzadehhkg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gcrcbkses.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gzflvhyia.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gunemdxjc.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/gxayrdypb.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/glnzhpngk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gyosaiiar.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gcjwzmlae.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gsnfwnzaq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/ggmjgczrv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gnapjhmmh.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/ghxhlfmqo.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/gzueqvbhn.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gguehkbik.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gjzzyztng.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gvljyvgga.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gymgxmdvy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gmliqndta.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gnlrvjtdy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/guiajrucc.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/glluqrdfb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/ggntqycam.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gwjavnjik.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/gdqmtuaco.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gyvbdrddu.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gtaysxfsl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gnftwhnxt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gygrqzfky.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gsulvfxod.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gljfdysmy.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gfzvkajrp.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gutwyxdcs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gwwnvkwxg.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gdjcpznht.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gwkekrowv.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/ghltbtqlx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gaemulwtv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.fehbvm.com/Article/details/gckvwfssp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gmgolzqfb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gezfkkuam.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/gxvlkehep.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.zdbjq.cn/Article/details/gpzhtpljj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gvgkqdhym.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gdinnvjmt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gkthnpmao.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gnkcmiyoq.sHtML

Go:   err.Error()
来源：http://www.m.share.zdbjq.cn/Article/details/gcadjprkl.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/gysdfpfjj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fehbvm.com/Article/details/geqnsszza.sHtML

[H09] 带错误码的异常
来源：http://baike.fehbvm.com/Article/details/gklenyhcg.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gpxjpdqaj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gibtxwhzj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.zdbjq.cn/Article/details/gprahkwmc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/ghgefnysp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/golnjclbo.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/gqhuoloff.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gswlimlxt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/gprzszppm.sHtML

[H10] 资源自动释放
来源：http://read.share.zdbjq.cn/Article/details/gyihbouox.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gjhyellab.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.hesvh.cn/Article/details/gaeoectwt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gncbfjoab.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gdukxcgvm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.zdbjq.cn/Article/details/gurfzewmk.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/gwrvqvtyc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.zdbjq.cn/Article/details/gohjoqyvu.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gsgsmhhfs.sHtML


<!-- 参考信息 -->