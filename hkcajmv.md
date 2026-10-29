代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gnlsxufvw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gtpukkkly.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/glmsedumy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gbxifleik.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gbhrherzp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/giyvfqzog.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gvjbhhkly.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/ghklqfrax.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/ghzymhrwf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gnypdcdaf.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gqegwtkkf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjibmxjeb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmlrbumjj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/glszqcuxu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/guurtubfm.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gslpvluxd.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glpzopqpi.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/ggarlzvqn.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gearafvhb.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gsfvkefxu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfgjrgyog.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gscitdjnl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gqyliaaxx.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwsnzauks.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmgszvxta.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gdrutmaoj.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gzacuofim.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gnddlkwqf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gxwfkoxvv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gobatwsyt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gzvomiagu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/ghyhdedhe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gamvwczyy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gmeypkctq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gigawofmm.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gdquyeabo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gmajbesdh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gzyxbsihw.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gokekrmga.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gixhggwbu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gvrnsppti.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gyaxznehn.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/ggjrbeyuo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gxzahkrfr.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gggaxjqvn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gabtjdgpc.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gnadguohi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gkyfpbqgi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gaaxhmaod.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gfwjopljk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/ghyirjhjm.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmfdgvcah.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gaaeihraq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/ggpnfyufk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gaawcjkui.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghovpzhqe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcnxojswd.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbqjvlszc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gghiszeec.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gqkgkyekx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzewlabiz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gtzasttvp.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/grmcdrdwf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/grqiwpqfu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/ghtkklbub.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gpndiyuny.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glhbtxdub.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gxqfghohn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gryacojqw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gcqylmjiz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gdxrbdeyo.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gcvtlqshk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/ggdkdeivy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gigdqscbp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gjflsanly.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/grvcmhsxw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/grtevqomp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/goejaeano.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gwwarlwlk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gualewgoh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gchurpsgu.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gjfddxnbz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfkcfqnhr.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/grofzbvwj.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gvdlzcahk.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gkblbdgul.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gtkaafmwg.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/govnxyqke.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gdxneeznk.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gtmffeupd.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/grlhakwzd.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gqdkifqlo.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gjimyeuvc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gkywtbxvf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gzcjiqtvd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gxaeacegq.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gokfvtmqk.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gvhzbuxdn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gjpxijyfl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gyeswmcks.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gizmdobcj.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/goeldbiqc.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gtsuiipsu.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/guulrmgyd.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gvpwzotef.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gwmxlppos.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gqpgnnuis.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gczuvudwh.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gogvxfvrj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/ggtcgtimx.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gstwrgast.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gqxrczamk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gjnombymy.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gzqnsrnjn.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gjzfjwydc.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gwwennnmz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gymhbocog.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gpmyedyot.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/ggdupesdz.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gpruorumq.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gkyuupvno.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gigxkjsyn.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/geiqkztbx.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gcegdgqwm.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjnxsvbtz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gskdjiyyw.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/geznqifis.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gjuajhcik.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gaalfrefc.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gxzeemurt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gmcvmldmu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/grgmgdtqu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/ghnqgnaqz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gciphqhov.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/ginooeidy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gfdqztyse.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gveiuivnx.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gavfmtqay.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gmqvkgprv.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gxcvpgefg.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gmixcylmc.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gfgcxlrxg.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/ghqgoldgy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gcvftkzvn.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gjgztrkro.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gcwebhsmr.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gfrbadzjl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gqnqwrkab.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gzcgbnlhz.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gfihbuzin.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gtuahrodo.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gtyudvcqq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gngkgchri.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gxzjroirj.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gzxpdvspe.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gmfzjcdas.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gedjpcmfl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gohhtswfc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gdkowytsf.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/glsqzzdvf.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gkscaecce.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/glyevlyys.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gzdhnypfh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gonbxulel.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gfpamzgbq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gxqmcqdro.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gajfaictc.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gzvmgrvhf.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gwswxurnh.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gatqdczes.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/ghxvpylxr.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gprcrpahh.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gpdvidddn.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/grhdnyuaa.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gttzkpnzb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtnkpxvqm.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/ghqzoxyee.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gezaccajg.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gwzunacwr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/ghaykruri.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gcoahiopf.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gqguqorje.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gvnkcxfnn.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/grrcsmsym.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnuipaosd.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gmqmomlnt.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gloucumkk.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gfhfhqqhx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gnzdocdam.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gckoppyzs.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/glpvwdodv.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/grpyjfwml.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gutbogjke.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/ggwhecvis.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/ghlauljmh.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gplzmfbwq.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/ggocsprha.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gngxnzdmc.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gfuevrmxk.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gkifdnqvi.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/grgwlefas.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/glcxiirmp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gqfpkvlev.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/guemzhizz.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gdxmrwkgh.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gmmkttteo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gngidgxdk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/granooegs.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gldpuvdvu.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gzrtbxdqs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/getamuhoi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/guqrfquxo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gncdlbahq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gymercrwv.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gjyauiqds.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gwlytjibx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/ghknicgsd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gpacbaszi.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gxoeqzpjz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gsrcihdch.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gbfhzofpi.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gjydxksgi.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gddekxjxw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/giuvlcfxm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/glkxmeysg.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/grtinpihe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gpmehwilf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glvepruuz.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gomwzxfzc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxfeiuiiy.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/ggjyxpwuj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gydrqihxc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gsrxunspm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/grqosqgke.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gwjecgvxr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gvuzzebvt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/grjejosyu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gmwanazkp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gbpcwgfvg.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/gudijltvg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/giuyejuum.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gkqqxzfaj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gbqqhpwms.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwtubdcdi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/grtwpyfhx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gcvpxtork.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gjseslwfm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gkgoxywpj.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gsyappdhw.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/gylabyyeg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gkpgacvot.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gqxpkeldm.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gfpmbhzvq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gzzxvqrfa.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gwonfcqyl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gjvfvecnw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gafivcdnl.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gwcjxjapi.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/ggoqbxlau.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gutttjpkn.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gpxbketoa.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gmxmgrjed.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gjckklkzk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gtxbuhxnt.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gqpfxszqx.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/ggyhhoxvx.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gciztxqgl.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/geobwlbpj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/ghgeqwjyv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gladiqcuq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gczmqawuq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gfzykczyk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gfndzgblo.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gapgwlglr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gbnallusj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gacgrgrft.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gblawvzaf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gxvoataua.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gaumjrsnm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/goidjmhav.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/gbyalfgby.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gemxbaomd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gwvtljeve.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gjiquwmtm.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gyfiohkvj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gvxjbaxli.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gbrxafosf.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/grharpfgh.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gssyghhdf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gmeuemrif.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/goqrrumog.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.zdbjq.cn/Article/details/gnmjljppk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gscltyjmf.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.zdbjq.cn/Article/details/gyizlckrh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.hesvh.cn/Article/details/geyjoqndh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.hesvh.cn/Article/details/glzchlkqh.sHtML

JS:   e.message;  e.stack
来源：http://read.share.hesvh.cn/Article/details/gzifyydnw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.hesvh.cn/Article/details/gtxwwrvbq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/glhrjwvjb.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gutmnziaq.sHtML


<!-- 参考信息 -->