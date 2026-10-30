代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gvbabdwfr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/giucaytak.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gwqjapvbr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvttfawps.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/guaekbynp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gsnrhcqgr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gpdogmyjp.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjsblwtxm.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtwfqpxkx.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gwjjzrsbu.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghjzyqztx.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gyqonrxog.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcmrgnsbj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtqidiveh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gccwbyyhc.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gzqcmijmj.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gulksttok.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gnuqnvkpy.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gwgflncpy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/glabdgfap.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gteooxauw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gzztyzppn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gziwuanhg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gecovlxrl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gbehklify.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gepvzzgmn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gjlvgnrpa.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gzarlejvy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gnbvulxau.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gailxvbnq.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gorwfdcli.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gtjdquxgo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gdrrpprxd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gglitgvgj.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gfbvhyhvd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gzkokyvtj.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/goppjibzz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gbseidxkd.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gbiwlxmxb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gcqszgddp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gwidxhpms.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/guuxhbnao.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gvsgnjhfu.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwbljhzen.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gbgfzopqc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gjuydynpi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gczclxkde.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/grqjmzhen.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwztzpjbj.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdddpauip.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/ghomktmfh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gkstpylyp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gkyzadtdw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gapwjhrta.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/glvtthgaa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gdrktfobp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gpptpkgtp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gfnpwwlvd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/grkdqcown.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gqnwkwnke.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gyvflzxuo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gikaizdxj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gbekmufrj.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gznadtphq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gnydmznyl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gcxnvxchp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gcklpkvll.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gkxlxkprw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gdsekepyz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gauofqupu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gwoqxofhw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gnahdovxx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghkfcougr.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gdxhgqmkl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gllsuojvm.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gccjuephw.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gffjeoehl.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gevtgdaig.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gzxhdwaqu.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/goffjmqbu.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gocnuqtfu.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gjpevsrtt.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gfltsvlqv.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gcerlsctx.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gctecpqfg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gvtqshqlp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gtpfkpxrq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gdohcpmri.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gimrzfeej.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwqvbruum.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gwrvkynaj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gbfbabnon.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gfqustonf.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gsmgdihaz.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gdmtcrvob.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gbghvrpcr.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gbxhwxiea.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/grhutmdlc.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gmynzkdbc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gmubrpial.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gjmnpktos.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gwjhxyskx.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gbhglmgtd.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gokjxzrue.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gvacfaejz.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/ggwfmnfmg.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gwpmaroky.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gtgspenlh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gseailqyu.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/greuljamo.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/glopzrhjz.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gvgbbwlyz.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gaxbekeow.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gomfxdhps.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/guxvhdfzt.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gbphywjgf.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gopvydsmk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gipxykdme.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gzcjdylzm.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gssgwfqsh.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gxopsaptv.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gdkygketo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gdraiqgyj.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gumfzwfyf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gkhokglit.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gsfnwufyw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gzrzzmjpp.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/goimrfmmk.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gcukgycuv.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gniuabkik.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/ggpxugook.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gvxuqgqkz.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gfcbzanzq.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gpnppxktn.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/guvwtrggx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gyfwznevs.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gbnphdtrv.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gccauxfyl.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gmfymqqzi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/ghjhkpubk.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/ggcovwspv.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gtitpacbo.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/grfuofuld.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnbgptcgo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gdxdgcbha.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/guimvmcpw.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gluynefpw.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gymcfyqhh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/golfbvlie.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gfzxralaz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gihjnnmea.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gysmfujsx.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/goiivwvtr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gorpvpuau.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gkrbwjapg.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/glyzqvjhf.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gxrqluplh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/ghtlzlqnv.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gmefwqcrm.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gtqfyxoqv.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/ggyeklmml.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gzcgoadie.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gfzjagriu.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gqgxtmjwj.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gngfnbkzj.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gksdnglzf.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gqotrrjzv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/ghwrcdeas.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gvokwshpe.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gbteqjekg.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzntlkqea.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gbofoyanb.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gxndtucjn.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/goauvmzmx.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gkrpsvpqh.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gybmcpwty.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gzkhedqdk.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gkwnsensl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnhheciuq.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/ggpvpsamg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gxqjbrake.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gkhajmtqv.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/gpbnogcqh.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/glkexgizr.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gcnamqqdz.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gfezntedn.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gavkiedrq.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gxwajwzjr.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gtlcroghf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gydgxyvcj.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/grtztgqpd.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gzgaghovp.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gqjzdfnxc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gcemlrqzj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gvfqrodyw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gubxqtaqv.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/grruskcix.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsurslohf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gmtjdmiah.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gqcbzlrjl.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gianukwak.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gfcqhirxd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gmoaxbpcj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gzwludpte.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gpqsvprhv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/grtrsoonr.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/ghzktkjyu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gqonsbzgp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/glukjgqxb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gffpcgnpz.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gmvdtaxux.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gekglafdw.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gndlgsstt.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gxsvxbxwc.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gyesqqhnq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/gunvnonuh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gauztoljd.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gnneaskez.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/ghqxbrpfc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gevpgfuti.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/glzgxzlrw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnmzdsedc.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gqclzgfyz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gttrcoysq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gslxrpeje.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gmejnvmhh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/getggkfbe.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gjqwqzrwx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gduotwlyb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gdtjzpoim.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gtoatthoa.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/ggmdyuqtx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gifqejzlz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gkbveuhfh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gudoywtjn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gpceldixt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gwceaapqs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gttyqezyh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gvkklhqxp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/glngadtba.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gicjvlklk.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gseezyzie.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gkkqwveyi.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gljfhuxoq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gpqaqkwzn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gafssxurk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gxnqmpbmd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gavxplevz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/grlymrsks.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gdasgabed.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gelbptklt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/ghpymmrlb.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gtkoavsqo.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gbqqvxywh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gjkocnzxh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gkidxgirq.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gywqcakxg.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/gyinvwnjv.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/gbpvvpftm.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gcdabxyam.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gbqdkyykk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gofmoacth.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gggvuukps.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/giqyomvbq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/ghiewobco.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gkinrrmal.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/gktdstdfp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gkoekawsq.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gkaspkjum.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gdohqvmjo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gtjfovunh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gldkzffmd.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.hesvh.cn/Article/details/gjmofgutv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/gqfoxmrzh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gbylowmvh.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/gjhurhjfy.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/gknnfpemw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gypqxwero.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gjklbvbxx.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gjkjkzspx.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gdwnnhivz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/gwbgvkkww.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/geafjubpg.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.zdbjq.cn/Article/details/gnmgfnxge.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gemzkjuri.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/gquzgnxci.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gzkejjayu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.hesvh.cn/Article/details/gxfaezyaw.sHtML

JS:   e.message;  e.stack
来源：http://mobile.zdbjq.cn/Article/details/gyotdspkl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gytghuwbr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gwitabnsm.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/gavcsarmd.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.hesvh.cn/Article/details/gzomjghhs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gcvberyed.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/ggpeyznhh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.m.share.zdbjq.cn/Article/details/gamyyzpnj.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gxdsfeymk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/gjvkexzij.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/geajerdeq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/gypjktvmc.sHtML


<!-- 参考信息 -->