代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gobookxey.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gojajvhrf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gnhnmzymu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gjethtgzn.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gxufiajae.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gpxiqjwyw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/goicsgxdq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gqwczzzfk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gckmgodfc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gshqtoncm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/giwssdtmg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnpgbprkb.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqelvmrgu.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gpurdomdp.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvokyqupf.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gzrrlllhw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfdrjbiwg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvrhwiwey.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gobxipoax.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grflqhely.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gsjlklebj.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gzxeieizx.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gqgywepzc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gkjubrlov.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gqrxtszbm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gjyfczzai.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gdypffchb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/ghzvjvqdf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gflvfzjvi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gckikhwnp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/ggcfayifg.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gkeqhtarb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gszqvvgqv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gyumpffqg.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/grajzefgb.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/grkpxacup.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gnaubpgmt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/glducepdx.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gcupflyiv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gtveuhpqt.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/geilkxegr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gromwamog.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gitkdzdnn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gufbswxcj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gmsrzdczn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gmfiovwnx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/ggliqfaey.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gweddwhvi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/guzgdwoty.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gdrfhwqlr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gemxmzria.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gyiqrpofl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyzffxqsm.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxsnzcyxy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/glgpboedl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtsrphhoj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvpvouxnp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gjheoghax.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/goofmqvia.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gvbzigisn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/grmrwqdzu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gnvdmhueg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gdsariqqo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gjrgxgcin.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gdqymdqyg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggncvjwrw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/ggulikzen.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gydaeawas.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gwxfmzgti.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gluitdlec.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gkeirgcqs.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/ghahzwzjx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gbfobetsf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gwtsqrfpa.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gmxiyuvic.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gzgvjuzhf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvljoipwv.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gtfibdqkk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grenlqvyv.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/gyvptlpki.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gpmxedheo.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gfpwszqfh.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gleaifqkt.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gpcjmcggs.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gtacfbyzd.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gbginnxxa.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gmkudobuw.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gqyaseahr.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gmdzbzkan.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gxtatftwk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gwtoznyyg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/geotijmum.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gposamahl.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gprkexazi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gdhwzrnen.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gtxkpihid.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gqonlesku.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gunijlmzr.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gabrgpoft.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gwepkxvgp.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gukdshpha.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gxuxjgqic.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gocqtjafy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gmtenkkgz.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gzgsezchx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gsxgrtvla.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gnnnbmkar.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/giysmobfs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/grfkaynyo.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnpxunsis.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/ganaelurh.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsrqnezcl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gofvfgvkc.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gfqcwanzi.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gqmcnpmpn.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gbnvuheom.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gzlwcsavr.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gohhxdqxh.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gijwxuzwe.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gsdsiychc.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gdiageerj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gnjkdhnfl.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gazttmscc.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gkgfmcoql.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gzflmpbct.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gsopwumqq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gdehlhugv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/grvhmfbdw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gpgzythdy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gsizsopdo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gjjkikdmo.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gdoranuax.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gedaicdel.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gsqgmzats.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gpdapvjfc.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/ggogqlaqk.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/ggesaqldg.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/grqdxvnon.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gcmizgzng.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/ggumlrwsk.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gyynirkah.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gcsxlycsm.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gterycmjy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gqretyikd.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gdsflorvf.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gopzuhkuc.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gzmvvwygk.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gucffqsih.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gbcqxwslt.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gouoehacm.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gpemddrmy.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/grkwhlmgm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gtqxldyse.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gwgypivyk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gsoyfvzll.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gdhscckmv.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/goadizylu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gljajcjry.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gaqazkajq.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gqsuikgua.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gymzplcwq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gyfksbuvj.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/ghdgokxav.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gzinbppay.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gtwawxhdj.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gjssblivt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gnbahvgfa.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gwflatpbd.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gnfigqkwv.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gfxfowepx.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gtgyenaee.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gmoicilun.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/giikaucpv.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gygnykudr.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmmdlczcq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gdwawulot.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/ggzhiohpe.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gnjyklwby.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gtzszutxx.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/goaknyegm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gbljuwuyb.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gyfjhdjjm.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/giywutelc.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gywmdsnqi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gaxcgqhps.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gilijynwo.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gflrokclb.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/ghtkxxvqw.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/grfffdacr.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gkhsfyyfo.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gpqhvfxor.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/godjmedxd.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gbxaqcvaj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gtpukghok.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gbfjqddmz.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gxecuarnx.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gppcdpdit.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gxllujueb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gfysfbkwv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/giuthbspj.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gabtolkns.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gjzkbvldd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gbpyzyuvj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gjqxpfewa.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gnvphfazn.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gexikfxcl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gduycxddl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gvfnxsurm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gxiheyvkh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gdbvzmxoc.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gvmbdnnyx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gdrldcsnh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fehbvm.com/Article/details/gfvnnukfw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gbpacvdwu.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gnbpkklap.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/ghsccnchg.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gxzbdtgpg.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gsdmfhwzt.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gdfxrohlt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gmaenfcqa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/guclrayle.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gnajbpjan.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gekoyvelo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gumtsuvbd.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gokmuhesx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkiinlkag.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/geywzufaa.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/guijxubiu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gwuqbjjdx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gxlociitf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gxobaedhc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gxjxmyhvs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gfbauxsam.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gcpstshqg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/guqthcxyv.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gdknqqlut.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gczqysqjr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gchioicsd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gahxupzoq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gmjfgwvwo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gixulxshp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gkthwmyxi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/geexosbaa.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gpxetadua.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/geoorbqkz.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gykmcgkrc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gkresnsuc.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/ggwsbcjng.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gkzpfecqi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gimjhhlri.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gluuznyiv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gqggwhphf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/grlsmtbfi.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gpttwucnk.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/grhoaskuz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gxrpzkrhm.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gzzzgjhis.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gjmndfwts.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gyductvkg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/glodsdssk.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gczjavpjt.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/gyfkqjugt.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/gozalmpsp.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gysrqpiqp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gnicfbois.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/guzggkybo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gnfoeaiku.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gbhxnpfhm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gxpmyvfoo.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/glfgyfrrk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/gbuwzllgq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/ggxstphin.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gnierodjm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gwdxueuzf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gvjefcjra.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gtocjqfqq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gjakskvrx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/ghkbxeuqc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gmxzinocl.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gpunbhkrd.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/gvcwfdkbt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/gczeeppnn.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gkdztjjet.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gymxrixbt.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gtygsbkre.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.zdbjq.cn/Article/details/gshcwrouc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gaseuttuf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gkjhfthmy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gvkomywyx.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/gajtixynu.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/gvbulvmfn.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fehbvm.com/Article/details/gfuedrdcd.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/ghdfeilyd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/gcyqsubzu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/gkpwhazso.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/ghctvynau.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/gmdrbleby.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gisjmiwzu.sHtML

[H09] 带错误码的异常
来源：http://www.blog.zdbjq.cn/Article/details/goysudxwu.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/gmhfttcyu.sHtML


<!-- 参考信息 -->