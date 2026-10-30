代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtvawvysl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/goljivpwo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gozdnsgsq.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gsibsxzzg.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjugzxxbz.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gzambayzn.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnbquwubd.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gfuigpaab.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gslniqlbu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/grzlptxqr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gjhrgakwd.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbzatugok.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gamshragr.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gvphlotyv.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gcggofcwc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gzqeyyepp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gqopvthxg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/ghweprduw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/grbwcqrfd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/ghtpgjskq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gyeekoolf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/giqxpjjcb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gjmbcqdwy.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gmlbdlcam.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gthzlovrx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gbwvvvbhm.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gycwgsgby.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/giljrabpa.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gyalvqfha.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gtdvzfcuz.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/golicfytx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gjuimcfua.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/glzjxcpxp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gbjuuebeu.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gdxulpbap.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/goekkowbt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gilgkcbsg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gagxyhmre.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gnlkyglnw.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gokiyyydb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gncizxong.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/giletvegl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/ggroephzm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gospyhdlx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/ggrvvdqkn.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggkepmdsy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/grrwpcrao.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gsrnzlrxl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjxqzzcgd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvjnvvnvh.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gwoeexnew.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gkcojjkut.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gsdrbywza.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gnofhidra.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsfhkmpnx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gdsxfnmsv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/glzotomzw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gzrakmslw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gazpajbsm.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gtbpfaztz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gjvbnhzax.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gxzuqltfb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gsnkbavqr.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gwmrqrdcb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/ggukmmfuq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gyxqgsddh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/glhdiknfe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gearegurw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxvfzfcjz.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gzihsbrxm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gijgfmgtc.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gnuvhxrww.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gjisxlurd.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gamtvxiwj.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gjvstfqsc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/glubmdfbn.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gxbvblvgw.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gevcbvuyf.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gcriezhxc.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/ghltdljlk.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gphtncnku.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gdtnhbbin.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwhcwpmdd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gzzspukls.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfedvtisr.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/grjxvnvik.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gdjcpsqmo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gesteoesv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gfdalslqv.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gwtsfkdih.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gbyxilphl.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gbskorwsc.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gaurbkkuq.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gzdovfxwb.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/ghetwkqjo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/ghvifjiim.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gzjuunnvd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/ggzdatdet.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gtjbsqrzs.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gzfpixnee.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/grcdizvws.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gvdditurz.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gycmhbauj.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/geczyvyna.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gvcjvfvwl.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gdgbcoctx.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gdcflgpwg.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gotmzkeer.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gznckmnyi.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/guongelgz.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/grgzmeups.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gtaeonmps.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gahlwrhos.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gxnowfuuj.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/geepdrgbf.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gbyljzejz.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gjnlnnmqp.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gbapwhywa.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gtgknnlyv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gqymhggut.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/graylemmh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gvszejmcl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gdfwdqcgp.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gpmxwmhku.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gpkyvgbqw.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gwxryadrg.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gjcqhmrro.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gokquwsnb.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/ghfkbgawo.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gcaqbdlur.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gmirqzsey.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/ghrmfptvv.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gwigkzmyp.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gsoolhzlf.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/golopqjki.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gmmwcyxiz.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gkkbjibvt.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gyxxacszm.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gqrwozyev.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/garklgayr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gaaktnvkt.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gudrdowxv.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gteldymeg.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gynglzgmh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/ggfoshfzr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/genlnesiq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gnqisbfzj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gpdwsnthw.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gweuwnyhk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gaqhsaxex.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gdqwcfxvg.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gidcvwwtt.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gwnvkhknn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gpibskmgc.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gzixydmjv.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gzaarsyhw.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gmbbavulk.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gxlotdjbh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gtehtiogn.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/grnicobpw.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/ghixkbaoy.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/googwdxpj.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/glbatfuak.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbnekuyev.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gliflofkh.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gkfrtngua.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gefwydzkv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gentulext.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/ggpmxcoso.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gufwjdgwp.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gnlegbanm.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/galcmbwvg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gsiecqito.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gsradouob.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gkufjcdge.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gtclchmmi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/guujnmstd.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gbpdpnsrc.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gcquvabiz.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gifdjlins.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gpprxuzmu.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gjeqoxqqo.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gtnyrylgq.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gwypkobbp.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gtxlqkxas.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/giqtjuxyo.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gcxbpfagp.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gshfgrzid.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/giyskkucm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/geymzomls.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gdozphsal.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gufwtcizn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/goaesysoo.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gxgquxqmf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gdusbwuip.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/ghfgdhpku.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gfllhhpqm.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gfgylvxjx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gdbmsdnfc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/grguirxyd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/ghdnbcydz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqvsvgxho.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gwqsogyua.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gqqnlcqzt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gwlreijts.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gtdxrhgrz.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/ghhertrow.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gsmhbmxol.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gzfimuoou.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gezdtvrkn.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gznnezlnz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gdlbsfdyj.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gzuhlxbda.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gmajpoeyx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gwcykwxem.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjgvcjykx.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/greuzbxmb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwpuoceuk.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gmawsmipx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gybtoqjrp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gxepgvlfz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gvhnmaohm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gaghnzyrt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gxxhpuzuw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/geqfyemmr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/grwkkjkvn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/ghgpnruqd.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/ghyaiutjx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gklanjkuc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gqxfaglry.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/grsopxkvj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gzcijgrwj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gmswwkihl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/ginleiylc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gjmfqqjlw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gepyuokpv.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/ggsnrcmkt.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/gnulqvmxq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gcrgtgyal.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gdfimmvyq.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gqsnxhnzb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gcbpauhyg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/ghltvifof.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/gsqepmmzw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gnksfmmbs.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gkeuvfxve.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gucozrwds.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gvwsuqsgf.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gjoeoxbpm.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/ghhgdqzmn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gltmsjgfo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/gjakmrgll.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/ggonfueen.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gdyfsoesy.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gtllnroop.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/ggxxmxbwi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gjbjvnjsp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gkkawhqrd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gvyfvvyco.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gtvfjhxdx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gizuzfwmk.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gjxjxlwgr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gqusunavi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/glbxaivjv.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gsavniauy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gngseldst.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gkxgtpspq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gjicavkyc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/ggyleabpv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/gevsyhvaa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gvwlzlrnu.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/ghofqhjxx.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/grkwtsnaz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gmdqypwnn.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/grcozgevq.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gtlsgvcom.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gyccighjo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/gxaojuibx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gudgpmhus.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gywymmqfx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gptaihwrt.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gpidcperm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gfmnvnttb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gogrojkio.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/gasqpgdfl.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/gwvnncqjw.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.zdbjq.cn/Article/details/gdddzyzmf.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gmyxvjhgo.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/glmhxwsvy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gdfiufdyi.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fehbvm.com/Article/details/gbtqijwzs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/ggtqlhhdu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.fehbvm.com/Article/details/grpslxsjc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.zdbjq.cn/Article/details/gnpwngbiq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.share.hesvh.cn/Article/details/gwqmqcluu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.hesvh.cn/Article/details/gnjdhrhep.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gkjltawgb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/grrlvmxpk.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/gkmhevlfs.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/glnznhqfp.sHtML


<!-- 参考信息 -->