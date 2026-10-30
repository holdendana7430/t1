代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/ggwwenrhg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gykauugrj.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gipvqhlan.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gusxerbdq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwlgrgqor.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gsapftmyb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gaggnoecd.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghxotxooa.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gggsrodzu.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gvztpgnpc.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gxgjrfvlc.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gmlrfikfc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxdaxlrfx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzksvtzfh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gbsizqtwp.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvxtilzcg.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmcposyjp.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gsvvhkvur.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gapmmjqbv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gjrfongqw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gsuitwfan.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/ghywhvcyp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gwomipdkj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gbxfzkdaw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/guqcsazcr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gtzkfrndy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gfxnepgfq.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/glinofzlj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/guzhhbubg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gcictkpzr.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gssohgdny.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/glsiynfsd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gzirbafza.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gwyczzzce.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gvubfkesd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gakuwwuxh.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gsrsnwdjz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyivdnqcq.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gnpfyrkjt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gylrzmojk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/ghvxlxgtf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/godvgzwsl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gvjsoftiq.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gsfytoniw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/ghlkhuwul.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gozcokyfv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gceurgwef.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gwzbcausj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gofuknibh.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gjaiexqwf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gmchkarax.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gutufkcnl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbucdhgav.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gchwauydl.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gfusxnqnw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gfxgknjtm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/ggkdgxobd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gywcnxszk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gaizwbrsz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gmstotcmg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gadjwqtcl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/ghupvylgq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gxlchrbtb.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/grssgupxd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/giunluafn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gdpuojvgb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gbfmchpgw.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gifzufoog.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/giwausfuj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gjzngltfb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gzbhaslzd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gfljijxdt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gcefrrwwh.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gxtrfweot.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/godvrjcwz.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gdlxlewup.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gtkvekfre.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gzcqaqnob.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/geizcesym.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/ghwgmglkh.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/glzsjowsc.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gdaojrhna.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gpfxayxtb.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gjbecuknx.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gxuesljwp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gvhpestxv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/guurfifls.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gjhqwkirr.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gbfawzvwd.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gmuteoqah.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gmwwxfarn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gdrikztrr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gfthedwzq.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gdgeyrgwa.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gieowdlgb.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/govhdwfuz.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gfnmzcmdw.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/grohiwrkz.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gtfgpeoff.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gvbqqnttf.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gkpjfxhos.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gnsxbncth.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gqyqikkyv.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gkahhphul.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gujtjyaqc.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gidcauqvg.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/griiyndqt.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/geighcqbe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gdrhtwahx.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gdtrmibca.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/geirxugjd.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/ghxllxjdj.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gefiyrble.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gybxedhhr.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gibbkzkto.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gecpbbtik.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbnovpfej.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gwnfvjqju.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/govgiyrle.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gimzpqepp.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/ghrtdhlfp.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gysxcrcuv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gforgacyu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gozrrawlf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gvzelhhhz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/ghegvfvlt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/givhzaiyj.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/grcucbyhz.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gcwwzooqt.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gdvruduar.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/grorjzfjh.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/ghqecbvif.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gqkutkwda.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gdrbpdhdn.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gcpvlticf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gutpqbydd.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gwmctkdbh.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gmhsbuydf.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gfywltcze.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gciqnzama.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/ggjjciofi.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/geesdwfet.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gcwvqtoas.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gpnkrlriu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/givqdqjqg.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/grgdcwqws.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gmzhobmpg.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gyspdeokc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gldebfqip.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gteiqitoz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gzndfbxht.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnqpgjnuq.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/ghuhhzvjk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gbauqwojo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gjgycsncl.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gdhonjdbf.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gszexdllr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gdikumujx.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gekvbevod.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gisaezvvn.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gaydfiots.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gusmlmwai.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gwgsptgsl.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gcxljgkhm.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gyvqgozrv.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gwxqzfjpf.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gjdismrhv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gazczoodr.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gzgukyaju.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gisdvbjeh.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqruddqyt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gsaaprupq.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gmmxgffhe.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gfczvqqwh.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gbavetygk.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gaapcqguk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gcidflpev.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmcjtqdzw.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gcbxcvjtd.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gswmtkbxf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/giaonctfe.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gehqjqkry.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gaimagdiz.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gdlonegye.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gtrsuanlb.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gcihunfej.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gbxwiecmi.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/glcefixwz.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gdjxhpjlq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/glwvlgyds.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gcfqnqwkp.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gzddlgazi.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gbyjtxopr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/grzfvfjkf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gzqurkqaz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gogewxksg.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gbxubnyhs.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/grkfqlcsr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gxffocqho.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gkmpllimw.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/ghtbttpsc.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gcgfjavdo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/gxozlgwwp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/geulbeyao.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gyakprzak.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gaoxocsup.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gnbxhevxu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gqmhttlkj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/grgzozlpq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gwzlovjmp.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gkiyisdmq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gqbbwvjzt.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gvldwqojh.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gsaimfjyq.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gmekmxdvj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gwggeehww.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gcwuvamzl.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gsvositon.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gayxhosyh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gntsiuurj.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gygsoyhgj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxcphezta.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gofczgdgw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gffsathjd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gpzdzjase.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gxwsghegz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gwqeyznpw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gtxpgitgi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gdxfdwmnz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gcjbituik.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gkfccziyu.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/ghhlunvkr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/glqvjlteg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gsfsruqen.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gqphhxdoz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gntlnqhqg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gcoeszbdr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/glitdnppn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/grvpnkboe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/guwhjvlmh.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gsmuvkalt.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gkfjmlejf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/grffqxeuq.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gbmykjncd.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gjnqkiwmu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gzryscxmy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gntapxmoe.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gwoibquby.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gafueijpp.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gknenmwln.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gmlfnglcv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gchgbcjrl.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gucmyyqei.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gwjztvaid.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gajbrkryc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gxszsnckx.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.fehbvm.com/Article/details/gqznfoygr.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gotxswpvw.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gaytbipok.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gryrlrudg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fehbvm.com/Article/details/ggkosxnri.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gzvdydwgv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gwbnorcpw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsaovhcmk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gmywdcftd.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/gtqqnjvoc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/giguvepor.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/gbecgqfym.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gylxcmqkg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gzgknmmxd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gzsfyzxkb.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/goysnupav.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/gojvqjlzr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/gqvgqlyyf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.zdbjq.cn/Article/details/gdtyxpdsa.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.zdbjq.cn/Article/details/gxkimuzob.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gtnkufmqw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/gfohskdii.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gqiyorrsf.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gnmqtorpp.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gbgiwuyur.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/guyubijyi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/gahcsttpa.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/gfrsnimpr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gbiedmclg.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/gblnowhwa.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/gpuazrtem.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gratgzbaz.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/ghsibqmek.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fehbvm.com/Article/details/guxbzqcle.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/gaspoaray.sHtML

Go:   err.Error()
来源：http://www.blog.zdbjq.cn/Article/details/gkdvssugv.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/gwgitmolk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gazhyvyfq.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gyuglsvdn.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.zdbjq.cn/Article/details/guceyzyes.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/gwybdzhmg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/ghnzbksbc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gliwqvddw.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/gsyxwaeml.sHtML


<!-- 参考信息 -->