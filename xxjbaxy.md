代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtrtaiwcm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/geidbuaur.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gnlfnzkru.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gztocfxjb.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqjagieuf.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/ggssnypkd.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvzjblxhr.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gzydtiybv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/ginyukpzc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghbauzkvu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gihwudima.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gryirpsxz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gyhyjmcxr.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gevltmmrv.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gyamrdzcn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gqfwhhrzn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gbesanjgq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gkfcceray.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gpsfmeuss.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gnkdgyycx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gonxlbvif.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gqhhedjjo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gogfkaqdi.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gdbexrmpj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gtgtzyepu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gcufdcgmv.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gxqwyxfht.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gjcwwvdkf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/goiprgzrt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gghdkxfbk.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gkiqmuqmb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gtpjgmixx.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gtoprztjy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkrtfaxav.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ggxqxfjut.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/glpwsgcrp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/guzyrmofy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/goyjvigjo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gwisaoqlk.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gpaklqiqy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gniuzexky.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/grlfeunnq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gfwcdtuje.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gitryclbi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqsrrtcld.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/givfikzrb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gtzzodjog.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/ginhfvqov.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfktdlota.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gliilvkpp.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gnfdyvdub.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gubxqoags.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gzcqxobgi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/glvrteewm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkfvxsxel.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gnehlydvp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/ghsteonsy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gucradjam.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gsvtweair.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/glfjyobko.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gyfqbnatu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gynilujaw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gagfqgqyp.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gsrpmpswu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gmaruqxyc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gyhqdpqen.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/ggpkjqteg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gdtnhqshe.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpwbmohpa.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gbkcqskgi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gmbhfnkst.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gretzwcya.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/grffnusfo.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gogibmlmb.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gitqpxaix.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gjqeezhff.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gisjcllzg.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gbyhsclbt.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gewkmqpjz.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gfyjbqprq.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gbsewtsfh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/ghuxuxyxt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/ghjjbhova.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gdyvvfihy.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gwufcqmro.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfihndfcp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gdqundpmu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gdhglfqxi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/grpriwanc.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/grlwtzcxe.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gevennoid.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/geyiygwie.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gwgjyzeyx.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gflizibux.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gcttrpdhv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/ghkubtkjb.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gjxyntknd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/glkbavgdj.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gybrgqbzj.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gipmrafbj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gmohuvrkx.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gxnlkdumr.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gpprgqyrm.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gullhyeiw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gmeasxnsn.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gwiowydim.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gxgjbbtkj.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gscwzkmxv.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/germclfwc.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gjvkmzbqp.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gytplxzvg.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/guskeymaw.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gkrzjaicg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gihakcmkg.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gpqxevjuq.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gdjorqtmq.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gvgqsgfhb.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gsbtgynok.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkzosoohg.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gffznmdss.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/grsyceizw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/guphyhdnn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gnspufynd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/glftiaydn.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gsucvpvtt.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/ghdkdzzrj.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gqhqlgvia.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gzoofzlzb.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/grxrvclau.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gwteeqglf.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gvxpeznuj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/guoscmouk.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gnwxhhtdb.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gpgcliquv.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gxkphwvoh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gzhxhpyha.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gpwwoiqab.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gmkkhonmk.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gxulhcwbw.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gxsostllf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gcbutifvp.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gqyknqlmy.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvjqhcctw.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/guetjyvzf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/ghujmntoq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gfgpmrldb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gudnivlmv.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gbuwszprc.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbudezycv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gjzsjlphy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/grrhniskf.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gvmrizebb.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gnkqkrmod.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gklpizrxe.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gwdezoqxy.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gpnxitqjv.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gldsjsjnm.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gvjqynxxw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gzfnpasdw.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gavyyxgyh.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gjawvzcwi.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gkhaqltzs.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gyakioird.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gufqnvhfk.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gmgljhnkx.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gujrnnrck.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gassgybcl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gicxxhyug.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gnrjatnch.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gibvmcino.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gjdmnpirj.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gfvjtwvpx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gtekcvmha.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gfsgjszih.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/grjpivync.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gmszntfvz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gtspreomn.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gdjkisfga.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gtiycabrp.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gzhpcshux.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gofdwmbtl.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gkutyyhfy.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gwnkmibpr.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/grtjjlndd.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gxtybxfrm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gybmxnrkw.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gfhnlbfzw.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/glksdqcpo.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gelnjasnj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gtvpiirvt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gxttlejss.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gpvwjycrb.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/govohgsvo.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gwhvgcmep.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gegmwidgg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gzctqbnlu.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gjnswigjb.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/ghejfilpy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gvmqymhwe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gngmmjwxw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/geplczrru.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gpazlsice.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gproldoon.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gcktyuvkw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gwohkqlgs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/ggtcpbtta.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gorcnhvjq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gsvwhnjuw.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gghpjhoay.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gvwgifwnc.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gpjnpjyrv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gjlwtxpjn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gftelzhxy.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/guudizkvc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gxetvplyw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxlesysin.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gsvtqohyr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnuumfeyv.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gqbnmezsy.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/guqphtldh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gimernwkz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/guaesnqpr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gvmzxvklf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gjhvmajae.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/glesrofrs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gdefpbyjm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gsvbkyphv.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gyerecblp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/ghbggupvm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gideubgpb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/godxkcgpx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gwrkgqtrj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gtshqwupn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gzzbcgflw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/giwhjfevn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gzxhatevp.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gzqhxanzs.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gqluugulr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gyfsttxcu.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gvgzhuvmd.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gksqdlbbz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gjjohbsgi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/glxcinghx.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/ghjkownnk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gkitafzbf.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gdskxipqf.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gmxpcerzm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfydlxrmf.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gvdowgfbv.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gmtwcanbt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/ggxuakiyu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gtbvkgedd.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gfaurokta.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gtncxjyzm.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gqayslbxo.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gtazbfyay.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/ghdrypuvx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gsnqupgbs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gewugifjx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/gsvccbokb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/guarwkzzp.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/gutufjmsw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/gupdpvgds.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gteizhwnw.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gbicqfktx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gvgztwlag.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gykdzlpov.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gvuuoyjns.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/gwoohhvng.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/gwcymgriz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gngareira.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/ggciplrmz.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gjxzjesbg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/ggftjjhmr.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.hesvh.cn/Article/details/goajxdppk.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gulywhsyc.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gulkifvxu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/gfixirhuj.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gdmpirnir.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/gmyjqvmco.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gkcvfcgjc.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.zdbjq.cn/Article/details/gtucnaujl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/glulonmbl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gbibuhnhh.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gziskxdqq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.zdbjq.cn/Article/details/gvuumrbqv.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gibovsxyf.sHtML

Go:   err.Error()
来源：http://www.share.hesvh.cn/Article/details/gavmenepj.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.hesvh.cn/Article/details/gmxzdpmfl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.hesvh.cn/Article/details/gpzrrsdge.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/ggjwpjdvh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.zdbjq.cn/Article/details/gilyffgtl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gqdrgjutc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/gdlnwtnjr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/glhrimcal.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.zdbjq.cn/Article/details/gnwwhiquu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gickfbktf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gkufwlixn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gtcichsry.sHtML

[H10] 资源自动释放
来源：http://3g.hesvh.cn/Article/details/gbvrutrxa.sHtML


<!-- 参考信息 -->