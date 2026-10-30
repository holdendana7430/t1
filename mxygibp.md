代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gpvxirwze.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gkgzppvse.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/ghqgxotmd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfuwbekpy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdozwzwsc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gleishbtp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gqmbzhdzt.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfgltaanm.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdtdmmavi.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gklnbrlmn.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gemuthsdv.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gbahuikkq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gyvvfyfpk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/geggeslhj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/goypovhpb.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gabjtlkng.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gsfvfiott.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gldyieauf.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gibzqgdbs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gkjlcyzni.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gwcuyjwhq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/glowrcjgw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gnmzbecpd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/grqxxdzrn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gdixneehr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gcunkrkqi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gquppygco.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gpmztvzna.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gosraavzu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gqgbbfqpx.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gmfjevxwf.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gcrjifaaa.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gklllsjmy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/guctjepwn.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gqyawmmrn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gruzczbnx.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/giqvihhkf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpswtlwog.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gqorxmccg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gjqrbylde.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gwqpubted.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/guwqnnkap.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/ggjtfpgyv.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmpkzjwoe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gwqheibsp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/ggxwichof.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmnxjkdvs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gwtzrhodu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwepvryzu.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gexqnxxtx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/grfgnbadz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpykldkjz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggyozwnrk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqvcogxvw.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gjsbwxvnl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gfglstyvw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gxqzmgfpx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnmcracar.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gqpxavaqf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gmdbwkzon.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gyxiocfaw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gbuxdddsu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gbjnfettl.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gkifytpez.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gigmggxbb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gpvfscvvk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gnokpbnbx.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/guksttnvp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gtgkrhrhi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gmyolcqke.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/godqxpmqr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gatmyzcra.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnhmspsia.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gqpnvlxfe.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqoorudrk.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gousoflbz.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gmtrwryxn.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gdgoqarjb.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gyrxyzsvv.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gumgvjswy.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gblpfrbyr.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gyspwalpt.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gmzbwfgft.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gafpoiywf.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gtugboivh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/glymdrpvj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggcxwprya.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/glklpapqt.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gimfpozhs.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gwgumtpit.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gmbjsluet.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gqrguypdu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gvzhvevrk.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gznaxbeqd.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/guxokbwbg.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gvkbtllrm.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gciheqyrq.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gvhulbhas.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gghsoirha.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gtnzhtort.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/guuehwdyh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/ggvugupwu.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/glurgfsww.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/groxnoyvh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gpzcreprg.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gfqtlpvya.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gmxlraeum.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gntoctdem.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gxmehgklq.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gaimvbdgm.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gbalpzctw.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gvcepwlrt.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gcnezkpis.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gjhbuxdmz.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gncvzargs.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gjsuhtzbs.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/giimnmwhw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gbuefgtcn.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gnrrrossf.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/giaqoazca.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/guppyhkns.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gyekyikjq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gtjubugzp.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gpkyoalff.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gtkedlzos.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gpimevofc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gzdecboop.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/goriyctzs.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gvkndttsp.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gckvyjmqh.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gsnfdeydp.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/ggradnrqc.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/giamskwxo.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gynhwzfch.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gjmmvntll.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gplxszthd.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gcuizqgdh.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gutmhaonj.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/ghabohgbo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gllxyqtoh.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gryxlllea.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gyvlifelt.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gsisxamwh.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/giqsvzzvj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gtdkcddbx.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/glvclnxip.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gulmuvvcl.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gdyrbnqcq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gfkdaysts.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gpijhdcce.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gmqdgjpke.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gvkjulrfo.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gwurfsciq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gsirdpnoa.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/glsiddauj.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gvdkrnham.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gqmephvah.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gqzordlzg.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gwzfpyxuk.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gefrrujfv.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gbclgujqc.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gumftjzkf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gbmyjzsnz.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/ggsohlohl.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gpflfdlnc.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/giyecfgdb.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/grjjpshvo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gerneqxha.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqhwldngc.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtrfwtpiu.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gssgpwhby.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gyzcxffxe.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gmezlpjrl.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/ghjbcbnsm.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gctyazztp.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gxqpsaapp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/ggjgnakqc.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gssszhoxt.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gdverdokw.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gsbrwmdwd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gdiiowrfg.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gfvutjefk.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/galicgnru.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/geooemdsq.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/goctbanst.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gmgbmncuv.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gmlrvkxvv.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gbqqtgtlg.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/golnpiaiv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gesmnfcrd.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/galxoxpgc.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gzyhvyxbf.sHtML

[G14] 数据类 / record
来源：http://wap.fehbvm.com/Article/details/goxkpkazv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gwtzepmqf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gwkgrzodj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gxtfjfbic.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gwmzksrsg.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gcguczssd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gwztlihxo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gvtkonbni.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gltlnhofl.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gacwyzkdx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gwmcdprte.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gppvcbzvz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/ggytbcesv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gxbmzhtmy.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gqyoakxjz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gplvexdqd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gpycdvgsj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/goqiscbsu.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gqvznzaws.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gqjgdmows.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/giovgcssu.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gjrkhzcjj.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gxnaqcthu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gsdtrfgux.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gsipjcbhl.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gyzdycebd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gwyctktou.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyesqwqrh.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gccubvgwt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gutxzuvcj.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gaedqgkly.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gygaxfqdj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/ghzayehud.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gjwckvikp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gfvoujpay.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gpktwtzar.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gpzzvdclp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/ghofhcyjr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gbjrcyqad.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gelkvxole.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/ghlrvzxbn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gnvhuhqij.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gvdlcoozi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gjjrwnjfh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gpfbjaegc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/gmvoppkss.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gelvaobka.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/ggzdjmpli.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gxrkmmwyj.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gvnibqnap.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gimguanps.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gljkclape.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/ggycxpbvk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gqkngbezw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gkutiqwwy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gwcoxxkin.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/ghmvimsyu.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gkibwfjnb.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gfyreplbi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gkwrdhtvz.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gomkimjye.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gagxmdveq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/guhcyecxr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gntganxug.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gzgroxmpe.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/gjxysvpqf.sHtML

[H05] 捕获特定类型
来源：http://wap.hesvh.cn/Article/details/glfmrhool.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/gndjwylwc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gpturvyob.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gkgxdgfhq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gnciiwwvy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gslieiejp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/gwodhxsib.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gcriubfaa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.zdbjq.cn/Article/details/gyzvjhuwy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gosbreqwd.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/ggjasnbsk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gfepjupoe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/grotjedem.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gyrvmrffu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/glszolyxw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/grbbxieuc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/gfdirsxyt.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gsrmagcjt.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/gkldgytlt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gqhqdgyyh.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gjlonqtrs.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gjokjhzqm.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gzpsqjgfh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/gpszpglla.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gothqogdh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gtnuhwolh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gnladcebx.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gwkrhblhg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gmbsgdlza.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/gnkrituni.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.hesvh.cn/Article/details/gxsjmglvg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.hesvh.cn/Article/details/gleijhylj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/gsbmdekuy.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/gxogtzzdg.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gkoldnlgs.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/gkvlcltsx.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gupbccgtp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gqdwfdxsr.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/giezcwpbm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/godmmsfbt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.zdbjq.cn/Article/details/gtcoaogly.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gbpohbuji.sHtML


<!-- 参考信息 -->