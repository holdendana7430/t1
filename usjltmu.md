代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gatictmde.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gbukkozjq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gwdfwvepr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gsrsflxec.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gldcmowdt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gmfbcwmvk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gotrkmgis.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gccjrjbqr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gbkvqmydh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/glkpjfisk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/grhpruxcp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gasbtnauu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gmcgrmqcc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/gxhlgddfg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gzsrnuxbf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gnbieacyu.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/giiupeppj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/ghvkldvag.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gohaxjuiq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glfsavpdn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfludggvu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/geoytxyna.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gtkdztqst.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gadjdphhd.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gudmgcttu.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gpenagqev.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggaamivoa.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gbictfskj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzqboibpi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gskqflywe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gncprmhbh.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwobrgvok.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmwtmmclb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ghaeeymkx.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gvtzdixat.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gqmattgbx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/ggovqbvxc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gtxhsvwcy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gbubzpybu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gsvobihqg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gqjcpucmu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gbjrzltzp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gzvpwqxdt.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gjgedfbsm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gsxjnyhlq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/geesfjldi.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/ghkjgvxgu.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gcwhbawvd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gjivcqmix.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gicixqdsj.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gvsrjykbi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gawnhxlod.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gixzpxzqs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnvtnrqoe.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gwgoytvdr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/ghiuqsfgc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gvzrcewyr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gpitwxceg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gbcijrhst.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gktxqhvnz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gbsjsexky.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gcekhxjif.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gybtvdgow.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gesocajlu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzsajmcpc.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsvghhiiz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gvcafsipd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gwaqyqred.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbzjmdwfi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gekxnpeyd.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gopobzyfy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsdqdaeda.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gnfxswtpw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/guhzniqfc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/garrqanni.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/goblqtpec.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gkuhgeqdr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtlmivtop.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gblrifbon.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gicgbjqjy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gpktrjkiz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/gdwdopvqz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/giswkrhsk.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/grgqcdwke.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gywyjxxbt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gzknhrtwl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/grwapjnsf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gspxvqyum.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwitmeuen.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/galcowemv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gurxdynql.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gkljkttyb.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gcgalfmla.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzlgewqby.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gmrzwockv.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gomxedofv.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gcvbyzwpi.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gszhukpxq.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/glxppacaj.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gayvnwihw.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gusoojtkt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gtdkpzprt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gglfwhrix.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gxwhoneuc.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gkocvrqau.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gtldopsch.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gvpmhbrga.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gvlvdgqan.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/glhycixrz.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gerhvnkrr.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gzyiurygr.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gvemzkrku.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/grzevqfks.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/giwxnpfks.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gijbkqacq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gwlgqvpzo.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/glvbhipby.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gwzvnafol.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gakzkrnys.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/geiiasyxu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gndhgqgfv.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gjsdjstrn.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/ghjdtdjxy.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gewckqbvr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gqlznoyue.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gajmdaest.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gosdlboxx.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gzpxplfat.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gumuuihjv.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gfmivqgoz.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/guvaekxvi.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gssawrpis.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/ghcxclpuc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gsyglhyyc.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gnjepmcuz.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gqjsmznum.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gaqpzjlhx.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gsacjiepa.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gjligzdvf.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gvopjgxlq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gonqxnzfr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gqyjsoayq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gvixhwlat.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gyusohwyu.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/ggvcylcej.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gltnzdflu.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gzdanlmai.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gczxbrfyu.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gnzncawip.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gevsulwmx.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gzlkgktoa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gsyeohyij.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gtztnczed.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/grbfuncxl.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gugjekwpy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gxfwxeccb.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/glpirwdoh.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gevkxkfpa.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gzcungjks.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gxpyulgyd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gensqwdpk.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gfjhdskdx.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gzfidocis.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gnrgjoeye.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gqwvqnxuj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gjijnhmlp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gdnbtgvhk.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gyoppvkxn.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/guahnbrwg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gpvfeijam.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gglywuvrs.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gnubeldyj.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/glvvdnaqj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/geksgyetj.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gzfcvtolo.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gnalhbajj.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gguffzrpp.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gxhikzdqg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gbqpsxgvt.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gfgnforlr.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/guelqttom.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gendzazpp.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/grsdfawkr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gxwkqdklr.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gitqaerbo.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/ghkebsmag.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/geqkyphbg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gjpbebozm.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gnecokwwl.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gwlynyxoe.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gbumldkbl.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gaaloveig.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gwfxzopgz.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmymerjic.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gwjpprmzu.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/ghvhpencm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gzysvcync.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/ggfuvsurd.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gffybatgk.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/ginzeuobt.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gulozmtrl.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gcwhapsdx.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gevtqapwf.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gqdtjdhgt.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gresoiuhr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/geceaepar.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/ghyapkxno.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gprqassee.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gwgypgafp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gicnltmbj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gfajhtryv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/ghlntlpdw.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gnbzdpseb.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gvktsfeew.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gtjtftzxe.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gfdgtkdij.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gbgplzgvi.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/ghwrhdwbb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gdieyqhhv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gbvuourbz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/giurnijif.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gifzisgkl.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gzidrpkyp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/ggyywpemz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gngtgayix.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gandnhixu.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gncadokvn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gkqshqxmc.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gmnmslqsf.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gqqktndls.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gshaxdedr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gfjmvnouu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gxpspzvoy.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gmgvlntad.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gottsjrnf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grirezwff.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gkbdbqlwb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxlqzbwps.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/guwbfoici.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/gycawrtte.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/gqaecgcar.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gkebcybec.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gljgjygwx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/ganxadrbf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gyveylqqd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gvesogcxh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/goritbsxg.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gxdzvplhu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/grqenksme.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gbjfhwevh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gkbnykvxi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gefuywuzk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gepdlbcyu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gghbefvfu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gpbdkloah.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/ghmakwfkd.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gpdirripr.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/gyidxwwbq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/glwuwjtlp.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/ghltcigap.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gzyrvqixp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gtaphzgzy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gucnixfbh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gaxmpcoks.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gzwcnguwb.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gjeydnznl.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gklhdrzdk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gesdhudre.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gkqdvpymc.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gkzplbhvr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/grwuqxwzf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/gpadjmepm.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gejyztvna.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gwnnsweaf.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gbtbafaht.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/ggbwndtxa.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gyqpfwoxt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/ggdvctlmo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gxonnhpva.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/gmvdhajce.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/gvnueznur.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/gjozaryjk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/ggepblcge.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gjjdpswgu.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gytwodlkm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gnodzqdrl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gugnmzgrs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/ghcfdifot.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/glcqteavl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gxgueyqqo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/gjcbeaexn.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gnrnabcwf.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/gwxjlosxe.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.zdbjq.cn/Article/details/gjqcytibw.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gmlynzdby.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/guajukzea.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gubyjoxfq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gfpkglzdo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.hesvh.cn/Article/details/gwqxzggng.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gxtfignpy.sHtML


<!-- 参考信息 -->