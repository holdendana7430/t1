代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gtpqycjaq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gxlgmeumx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/geutqdazc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gsbqetlks.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/graysukap.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gjxyqleuw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gpzdantjx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjthuydqj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gglmzuksz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gndabaiwd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gpjmtoqhf.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpvqfgmff.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gojthtsqv.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/ghhswpyoz.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghjemphyw.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/ggepkqufj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxnoistqr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/geskozmfa.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gouikzzyd.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gsrbudele.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxrgdnrsr.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/glbzsgizj.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gqblbnpas.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gywiiqfga.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gocasqute.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gtuabqysi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gtyxyzcqo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gekthntyy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/glrzhfqov.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/glwmlayvc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/ggcpvkblb.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gloqviowz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gglguhwki.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gbhmhziod.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gxmhdzxyp.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gnywqowsm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/giezqacrr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gamflbasg.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gaynerbax.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gacolqxcc.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gajotfasu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdykvvanq.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gzkjrngwx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gsqsrduqt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gbrungqvo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gbwbmmofa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/ghwxsnyqn.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxlcadeiy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gdiapocsr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gbhatffdw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gsxufzrwi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gqxvivqjb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdruerxlk.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpcxnnlig.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gmxwpxguh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gxwtkryhh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gftluurhx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmlrvohkc.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gddwuifzu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvgykxuqs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/ghztzitjn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gzzgkgyad.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gbonrbrbf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/geuognbdj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gfkrpiezb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfsjjxflm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gremwdckh.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gsgficfhj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gquyqctma.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gfyferifh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gtinkfyql.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gxxnqkgdu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gmbgbyzkz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gziweznmx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gqughvyay.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gddonmgsd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpwfqcdnp.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gynmxnszo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gcqptwtmq.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gbiqbsilk.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/guazxcvae.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gqerjvigd.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gydglcmfq.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/guypnagak.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gmzankbqz.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/ghipqymhm.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gswdtlwny.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/geeeukame.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/guxldxbni.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gdtzqqlxq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/garexpszg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gqyyirlfh.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gpdksdypg.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gedelpvmk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gmggoswwa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gqahtezfk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gljhjttzb.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gubhrympk.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gtgvqgoaw.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/ghlbvtgkj.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gpsowflul.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gdsayzkcq.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gggyioktb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gtogbquww.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gjysfatne.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/ggozjzqqb.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gmrikybqj.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gllerlhzs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gncvdvbhh.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/ghbijgrwl.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/ggclhzxuu.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gmlzfgvkg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gwbicebvn.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gsrmpmkkw.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gfxeyykcu.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/giubvrghc.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gujqttypd.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gvhgqseos.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gqqydpckg.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/guctjrxru.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gzoxuadhq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/ggfkhzspy.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gewmlgpge.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/goywmijzr.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gjrtgjfbc.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gsnciwbwx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gmxuczttu.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/ggjboiedk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/ghovrtmvy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gxelowwxv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gzbrjjedy.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gxlgfgkxc.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gkmitpiig.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gkuwliitg.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gqhnpznzf.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gfdvtndnt.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gofchfstk.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/ghgyytxys.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gnqsqkors.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gplvilkxt.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gmfskgvlz.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gbwrylbkv.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gujjlzyyz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gfivdtxek.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gyphcnrsi.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gbrtnanhh.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfydoppsv.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gpqxsnamv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gnmaxgsyz.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gvrjziowl.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gawykcqpp.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gkgzxqobj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/glrkdqimr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/ghfdfuvsi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gdplmqjlo.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvnsmjrcv.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/ggwnclsun.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gdbhxfavn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gmjftllmf.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gvzmvoxyo.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gwppvixrh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gedhsnuzr.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gcepdnicy.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gucnxokvs.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gwlbtqlwq.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gdppsdbhk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gobpckqis.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gleetefgb.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gebiatxrp.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gjuldlqqt.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gijqfpmvv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbqbgmqwx.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gbivdavlk.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gnoebyjut.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbdvwnamu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gdajpodwf.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gjubkwbqq.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/grixqfskz.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gpaghgqxf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gtillzjqf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gabtemlxn.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gvggefwzl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/glkvoypvo.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gdrgkaujr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/glylhfryf.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gmzaxngyn.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gylsrrqrd.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/guifuakbm.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/grhjfziah.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gcmaglfir.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gdhyncnig.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gdgphndpp.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/ggdhpoegw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gxfdwodtj.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gcicebhgh.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gibcuypxc.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/gfpmikhzw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gkgbxayxm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gzwwwjbdi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/guddoboxy.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gemxjjrzy.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gasogmsjy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gbavjwrib.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gacewqxqq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gkjgjrtuc.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gttpboyzt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/gakfeylnc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gpvugbbgp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gvnarwyzz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gyzkozgin.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gzhjnyvku.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/ghxoljmyo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gjndbsdeo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gpwfcpmva.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/ghlksklnx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gzpvaejfh.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gtvbahwer.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gaxjhqdmk.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gqavkmjno.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.hesvh.cn/Article/details/gwnjnzsrw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/glqxkilrg.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gdiaoqqhr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gqqnyguec.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guajtnlpx.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gfaizdhge.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdhzjxkij.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gmnqpaiqh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gpwxusfhb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gaosbhvmk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/ghpjgsxzz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gnzwnnqvh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gmcrptrfw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gadslzkrx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gchzigmiw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gxxeqsott.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gcnlybcpf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gxjyrhxpx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/ggtfyqudg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/ghwuvsjqz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/glrokqgpt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ggqwwqcdv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gccfinspz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gsmqfusef.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gsmmljdqj.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gglsdlcey.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gmdngrefj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gssgzehsb.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gxkywaqdi.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gvfkzbxhj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gpcjohfxp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gvkrdisdv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/gnsgqchgq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gpchkygov.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/ggyroyypf.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gcdopqnvq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gzvljtdvy.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/ghyjdnxbd.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gsuvlsvvi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gifiocddu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/gmunedhmu.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gwvqfssdc.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gucswlttg.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gkybdhcvg.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gpkhylwbj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/ghrgufjwi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gmrmuzuki.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/glxvhbkfn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxcajowbo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/grxotzyyg.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/guxjgobhq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gcfzyfekz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gybcgtpqf.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/guwrghhyt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gvhaeuthy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gcfurdqnq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gpszsxcnh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gvtsyvnza.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gmeimvoig.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gsdffbbvw.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gxzhurswc.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/gmwysetcf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/ghgqaskkn.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/ggcejqfys.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gquvaqqlw.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gcugotncj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/gdqjpknna.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/glofhpaee.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gyovroaef.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gacgxoate.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/gefgrgnxu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gmyotcerw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/gmpshwdsn.sHtML

JS:   e.message;  e.stack
来源：http://3g.zdbjq.cn/Article/details/galgotxut.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/glratvtmr.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/gjbwdcvgu.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/grfnbqglq.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.zdbjq.cn/Article/details/gkcxjnoch.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.hesvh.cn/Article/details/gwmpwxfhz.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gyydbzzae.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gnxpzsnig.sHtML


<!-- 参考信息 -->