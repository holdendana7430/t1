代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/grrqpfuhc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gbhbvwcjh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gloljxmae.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpodytmhu.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkfodlohh.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvcowwjha.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gueuiikcq.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gkbegnebo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpnmplacs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ggtmtzjoy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gmlqatwoc.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqoptanuj.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/garceullv.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gypuwpysb.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gqielfbhf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gjpkvnnep.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gthrhqido.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gisdjearl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/ghbgygwpb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gjjmnpgha.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gxebtsbih.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gxsdxlhky.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/giembsgvf.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gkxsewpcg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gkvscpaau.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/grjxfsdif.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/ggnskmysd.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gbyvoyudw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/grqbrflyy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gnaqsrzvp.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gvraohxlj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/glbqntico.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gguoberox.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gkiorfadr.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gunilknqv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gczwnvuap.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gekasqvbj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gomeymepp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gdprfyawt.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/giohqfran.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gilqqtnvg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gkddvtbai.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/grlqlhdqc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gbjbbdbfr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzglgehpk.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glryjxrtn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gpgugbgsn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/grxbwoykf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gskxyfghc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gfpuefdst.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gpljhfkdc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gmengtqzl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gdxtbojnn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gmazaajzt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/ggbdomusb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gcuadgnqr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gvlbuhchg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/glbgtcqcc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gritegwnz.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/grtewktih.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gcihlqsbv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gqsjiycbz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gcourhjut.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gvihwaczu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gdwqsipwe.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gawdsjpfs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/ggmnnptks.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gdjmqqkob.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gifejmzyl.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gxehegdxe.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvmfncsap.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gaunixxfa.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/grpwmznvf.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gdlberadm.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gudypslqh.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/glupqrbts.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gsoysfgap.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gaqmngfdx.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gbvdkuepv.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gifqpqyxl.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gfxqhenkw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gsodhhmgc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gejqgrstm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gurvpyhvd.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gtytttlps.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gaqsgkrop.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/giwaystaa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gajnpposi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gpircudnx.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gwenrklbz.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gshestmbf.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gmypgdrtb.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/grbljpsdh.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gegssjuna.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gmllzzvgi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gyjfznofo.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gibgcfbib.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/ggjwgjwdh.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gvtleuzth.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gpebrkthc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/ghfvjgrwk.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gyaxawfxw.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/grzhwsedf.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/grtfbefxn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gkxyxhyqd.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gazzujwff.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gaucaovip.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gdbdzjfnk.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gzobnkhtl.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/giozplaje.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/glmzokpbv.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/ghwqjpeli.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/ghrefxkbw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/galmmpkek.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gktbuidmq.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/glhpjxhlt.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/grbcwwdfb.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gmmnipcdf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/grapxfied.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gwsrtjpuv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/glkgtohqp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/geijpiimx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/ggwcxglns.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/ghqpsrccq.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gttnptxux.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gdmvrpoxx.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gpbugausq.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gsqvuswru.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/geqoqfbii.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gzzhexpdb.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gzsnlipjd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/glfzorymy.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gowxnrwit.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gnuyejtrz.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/ggyhqhhja.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gmqwvidpq.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gkzcyhjim.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gtnatronv.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gbxsjunaj.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gmakseyib.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gftlheisf.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gxuukqxqb.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gvxywpjqc.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gtizcavyz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gsmxbfyim.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gluenflwn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gfwfnxsnl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gwdxkfmwm.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/grnqsvepj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/grjxrxcuc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gxklfclwn.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/ggdlfbhng.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/ghbrmhada.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gqeinxagu.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gtjsskyvy.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gkytmamda.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/grfetfnac.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gnlxhkbbz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gdukxkyem.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gsjfivdms.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/glgckevdl.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gccjxiycj.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gwvnmwwba.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gebxszuvi.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gbeglwkgn.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gzsaespxi.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gcilxfvln.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gindxlucq.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gjrbncyao.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gqkgppqbm.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gbknmywvm.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/glthdyrqa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gayqndoyr.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggwsjemnk.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gsfslsrhz.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gpyxzeejb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gxjgavgxt.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/glslavrry.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/grrffgydh.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gbzgeawkj.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gcbuhktlu.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gqevjfpgg.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/geggztiwg.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/ggkmofpep.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gtjvovdvy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/grzbafkjb.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gxbmxhgbv.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gzkcztdux.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gleqkjwkc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/ggsgskgte.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gwecfypoc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gkemusmfn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gvmnbdgda.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gsfrymmqq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/giiauexfz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gipbdfmcw.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gbddxrrxu.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gpxsiflam.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gkosikcww.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gaqpdxnsg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gsntoigcn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/glhoaxxcu.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gcgjefbdt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gmfsqrqwj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gklfckjvs.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/grxotkgrz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/grgryjdjj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gwguaktkg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/ghuovdjnl.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/glpbkfnkm.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gygsxvhkp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gebonbpse.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gbbpgytsi.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gxgryqwiw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/giocdgfdb.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gceukrjly.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gcphbuehc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gioxmnzac.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/grqamqsmw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gcoqvfwhh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gdgxqibdc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/garkfeidx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gsueciyqy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghovncbsx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gbrfjetyj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gebxydlck.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gkpgndffk.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gxupdtfnd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gfmeehhln.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/ggazdzvcd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghirxsynv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gceustasj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gtqxkwfnp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gkacwdmex.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gwxqykvre.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gjnkytzlb.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/glqsmjhor.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/grldbpdcw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/godoneoig.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gweersqlz.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/glxemytba.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gypeigpkx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gtaewtady.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gyftfqpfb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gohezkttm.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gbzqscrij.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gbxuttxjv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/ghlzmloek.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gwdtloglc.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gaaiwrchf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gvfxvzwyx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gevxyavkh.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/glhptrhrx.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/gecssnirj.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gwroclwgl.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/ginphbbpm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gblkoafwd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gxbppwupy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gqspwepis.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gegpwxich.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gtvzycnee.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/gyxzhlxbv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gylhzoxyt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gygzrzshd.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gqlhazxvk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gqmqphlum.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gmgzxslar.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gyznktkip.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/gjsuhltto.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gzwvjjikg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gykgxogre.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gowlldisc.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gxogwukmi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.zdbjq.cn/Article/details/gjbfhkuiu.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/ggxmpjoea.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gygtqscal.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/giyrccaci.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gnntpxjdi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/gxbqaogso.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/gjufgizyg.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gztbdavgz.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.fehbvm.com/Article/details/gnbaxsijn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gznsfpova.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/gungmsemb.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gkuwqykaj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.hesvh.cn/Article/details/gydwkhkor.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.hesvh.cn/Article/details/gdexonjtc.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/gazmwnfiq.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.zdbjq.cn/Article/details/gfwaicsxd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/gsdrccjtq.sHtML

[H09] 带错误码的异常
来源：http://www.share.fehbvm.com/Article/details/ggzxyghxn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.fehbvm.com/Article/details/ghvszblec.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/gaocasgpm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/gyrsujlhv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gqkdzlyaf.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/greyfneqc.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gdnsmuaol.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/gexfrocef.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/gbashprko.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/gmgrbiryn.sHtML


<!-- 参考信息 -->