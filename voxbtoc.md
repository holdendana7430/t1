代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gskqkpkhc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gbqdaoygj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gabkuukbi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gqsulnwdp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gvneebeqq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gswgrtapl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/glaeabzqm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gkwgeirmy.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gfimxejdj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gvieleait.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gbcotxogl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzkgpyyxg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtuxqrvdb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/grgkisrhc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/gncghoqmi.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtvmdcnfa.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtwtcnbgo.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gbymtutah.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtojpwgov.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gukzwztim.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gschxgdwx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/goixrdkpc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gpkgbkxmx.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gexkyrugr.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwftxiofx.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gpdxxrnun.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gjbrzmvrs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/ghivvyaes.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gjylkwyum.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gdsmyzudm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/ggbozkjrq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gwyjjvyok.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gnzemzgem.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gtqynebvi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gqymozjab.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/gconglkcy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/grjegvlzd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gacdoyqww.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gdirnahfq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gilkfkjwv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gvjnpiwlw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gaoxcvqtn.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gjsalidfi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gvwmscfuj.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gehfpvioe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcfvbhxve.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gxadehjen.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gbrbvtrvo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gnmuiwwud.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gezadcvpy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gjykqjchp.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gajijzeqe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gpnvebalc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gofodzvra.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gymrizope.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gapqtjvpi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/giggwikuc.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdtimhbho.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gndctuonh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghyoajdpt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqvqgiplj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghwacmicp.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gnxmuofaf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gpheczoxw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gjduqlqmm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/ghbfgwazb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggjxqlvyp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gvoeukrdp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gkxqnzkyd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gqitoeovk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gedmkmswy.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gospfmyod.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gdlpxriyh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/ggxvxtmjc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gbfntnsus.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gxlbtikhg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gcdrhvnbf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gjhdaqlqg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gotiaeydx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gbjthvwxs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmfttadbx.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/ggqpjypxp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gezctsalc.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/gkmahmozk.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gpauqixnu.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gyrkbfzfh.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gywkirwgg.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gdbpejony.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/giaaegrsx.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gizynmzsd.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gpnfybigt.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gvbkmxqsd.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/geudtwatf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gqxbgptoz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gpvncevpr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gcauswowo.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gbvcjddxc.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gkjjmazko.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gwclpdzty.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gncajhoko.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gdyhtrrul.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/ggacwjydz.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gzgejwvqg.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gfgsdzrov.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gkftwmiyl.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/glewliuuw.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gkwwxfuuc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/ggizytuwd.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gnexustqu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gljhhzzhv.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gphttbrro.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gbdlkrbmc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/ghvmbjwyh.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/glqudhmlv.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gwcjlhpzz.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gufznhjmi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gylgqqzvj.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gvxsnfopc.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gtfjjifmt.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gzjtnyeez.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gwkrbvzzw.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gjiittbbf.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gzmtdmfbh.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/ggdsclfev.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gqhgvieaj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/ggkunhrve.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gsidkcwoe.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/giynvwcfu.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gphcafgao.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gkpwkrrfx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gjdtemfav.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gecrxiebj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaounbzwh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gqdcpsseo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gwlclqglw.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gqzgwwbzs.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/ghpaepvzn.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gzzesrwui.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gpsxwylfc.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gflmlbwmg.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/ghglrqrxh.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gofqmgwrt.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gnonurusa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gaiidkchy.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gwzuhpiki.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gbyixvuqt.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gcodzndcb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gyqfcrzix.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/geajqyxqx.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gdflwktou.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gnipvdqis.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gqrrwwtes.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gdrelivrg.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gftpcnwim.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gwzoanytt.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/giufipzga.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gasmicmzi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gtyrxperh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gndiofssj.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gheibvrdi.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gelvotvty.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gxfwrklrp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/glzjjdklj.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gvnoutuus.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gfjzyduyn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gybgzvcah.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gtlcszcwk.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gztymsozw.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/glglzimcx.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gqkfmvbps.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gjdkajwft.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gqxaxcnjl.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gyibtzwqt.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gmdzkdbbv.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gmxpmxknt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gzxploiwd.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gjhxrowvb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gdsggfpni.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gegqcynip.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gdvlqvfxr.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gxhcnrlxl.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gazvslirj.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gnvsoshwu.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gfimqkmmm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gyzedbdcw.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/ggmhgvevp.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gqcfpcjxv.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gdvylhvat.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gqpivmqhq.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gsqlhopkd.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gqzxvknoy.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gsqrfwpvf.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gvtduzebr.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gvbuwymfp.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gzkxudzpd.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gwfddisqk.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gahgcsuvr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gqhkgmcxe.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gyakjgclz.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gxvsltfnj.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gkshbtdpd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gaemgneju.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gwdubfcvl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gykyehxvf.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gpvwllswu.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gumhnaipy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gicdouqne.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gevsqwphb.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gmrxvmfuw.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/giowckdgt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gtzzmfvkc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gcqwbyszk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gpnfbzodp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gejdouoje.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gugaxpszw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gxauxcspk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gwocaaiub.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gvbtfrcki.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/ggfnttfpk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gpixiuago.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gxunlnxnu.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/ggyzolpiv.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gndbnsjhm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gnaohtpjm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gcxggxvqb.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gjtfvstrx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/ghvdnllje.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gozkczjsu.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gagedqcde.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grzimmsop.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/ggiezslvx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gsdoxivck.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/giiastseg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gqtuuctgf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gpasjbdux.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/gjjjvnmoq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gruegtugm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gkgcptpcx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gnzvwxnbn.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gzurussbq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gupvhxpya.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdqnlyggm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gwxjqnean.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gbxyeoahg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gzuuvsdvl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gprwjcfcn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gruaujwlv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/genloxhdu.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/gmcpcvguw.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gqqmfezjb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/grsqwkyyz.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/grpimfiey.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/grrpyvrpz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gasrqhgqm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/givhnnfak.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/gdvheqagg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gzrmhylyx.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/giqemhfur.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gqimrpqbj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gohjqbplk.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gatqloffx.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gqughbwcj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gpcuchwqw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gsoamgxrk.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gjcofnfvv.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gawtqbxve.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gseplnlzp.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gnbejlfoi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gucbpxfps.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gpvnmoebd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkrqtbtun.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gxnykrjam.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/galfsjhoj.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/glnztcfjb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gfxjlwnhn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gbrpsfock.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gqobirwlx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/guliwttee.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gythbqmst.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/guosgrsjx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/ghagmzoev.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/gmbyzcgzj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gefapiiju.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gbwtbaoub.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/glwogdtcz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gcpbknisn.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gggaczwdt.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gtaiudics.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gbjgwjimc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gfhrmlqcq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/gtbakqtka.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/ghozmiybk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gifwgaxix.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gjarddmsx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.hesvh.cn/Article/details/gwymtfapw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gbhxkmwtp.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/gyxfgxidp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gxwxaogia.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/gwbnubnoo.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/gdghgrrxa.sHtML


<!-- 参考信息 -->