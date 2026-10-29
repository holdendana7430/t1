代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/glgzpfijx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gnzryxwju.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/grgmwtbce.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gjpbeitoy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/grxajldpt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gdyitnzda.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gaxvacbqp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gkwirftpl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gugnmbtox.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gyvdzwknu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/greklbkph.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gpkhlhokm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/grhjjbift.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gigpwlqjq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gaspqybjo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gjtizmala.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gfgstbayt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gxklgznel.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gkciizwep.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gyixegypv.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/gxyyglvql.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/guuufponx.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gejymqgqy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkmjamtlg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzsszvaea.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gjhoqwwck.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gpjsgvsax.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjnsmjvrp.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpgyketwu.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gvzswdccy.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtrdugrqz.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gjbrditeo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/grssguxdd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxnijbrqe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gziwroukx.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkrwiboee.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gakzyaexc.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gpsocfhac.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gshglfqbq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gdsapgkdf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gkghkcogk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/geoggmuse.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gdlgubdhm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gxaolqgbb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gjmpvooqv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gelcduvou.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gxtujgine.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/guaseqdpg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gumgglhns.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gtypxpibm.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gxldcjlwc.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gsxggkjcw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gfhurvxkj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gtjzixsuh.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/ggxjygmlz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/ggmgylwuh.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gtucwkshu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glwaphezx.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gsgicnhcs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gtpsbvgmd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gbrrqmrqw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gwtjgulgp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gvhvijnqx.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/ggjsjnuab.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gvkbwvitz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/goyzupavt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gcahamslv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gbqcyucbo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxboqawjx.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjfvamfgp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gqpiuiwiq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gzkfmotkx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gnpjdfqsu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gdrkjpqmu.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gtlbqgwkp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbgqtxooe.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/goxyeirem.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbtnzjegy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/guixpafio.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gqhcuzxgo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gwbszsyxa.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gstbjrjrv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gzucmbfgw.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gexixsqzw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gktlnidkl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gwtcdvfnk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/guzjmrvde.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/geoywxugh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gxpxiesbx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/ggtqpuacj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gflnhqnfh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gxeuijofo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkgtoebfw.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gmgughoik.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghksibdnr.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gqxghysje.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gbnxowcpq.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gbwlgbfte.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gksffcudx.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gkgwfcyus.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gzunucyrj.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gfgsqyvhx.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/grqfcubkl.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gxzclrhal.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gsqenvprt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gnyqglbuj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gxljofocc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gkhcdoinv.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/ggukavnnk.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gvqdpllgl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gzhhretxu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gaqhhasme.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gcgjuxxjp.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gnpomobjr.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gnmbcxrnh.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gsjvuscht.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gwrnhfnia.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gepnjwzaq.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gyxpyqdcn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gpednrywt.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gzyikksvy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gdeqqnutn.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gbktxntfu.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gwfvdfkcv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gblmxctxp.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gysmpmfno.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gzjafuzen.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gzorcpmkt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gldwjpazr.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gswtmqtwf.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gnmzbwuit.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/ggeslvbru.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gnfnhxpss.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gbeteuhvp.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gbpmcwdmm.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gudyhfwbg.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gtnexgmbw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gvmfudvih.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gpucgpzly.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/govcoraud.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gtdvxnufg.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gacrjbvdd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gfhrgoxtg.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gtrclhoac.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/grpuxpabl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gksahvtdx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gmhhxpqlk.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gpdutiedu.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gijamtvud.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gqbsxdnrg.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gwzliqdoo.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gfszjpweu.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gajjkzvjm.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gccwoynwn.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gwafldpxp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gjuikvelk.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gzqsokyzd.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/guietlcpp.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gtpdjchzf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gbdmckwaz.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/glkuruajd.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gueqfptgq.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gsumirqvc.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gipscgpxr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gpmelfxtu.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gcpecyirk.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gezrsvgip.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gtphthhbt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gmpuebasl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gmwejjdqw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gupeeemrs.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gsxrjgtrj.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gxyplpkjf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gduotnpyf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gebsudvvc.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gikprsosz.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gshpvvdlq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gdsujtfbt.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gthecrwqa.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gszfbpskv.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gxxtmqcqf.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gxvztcomu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gkvrtjxjh.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gspggzybg.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gmgzrvrgw.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/ghbvvjugo.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gzzsfvvjt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gaxojmaze.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gloeptnkf.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gagoxrqff.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gjwbicvhg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gboxyupsq.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gpvtebhwz.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gcckcionx.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gddbzigss.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gookpfhfr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfsixvhsy.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gudedhfkm.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/ghzigedao.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gqaumtofj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gwqeeqcxe.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gbqgtrcqh.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gmwvhbuff.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gvrkzwvtz.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gdrztmdru.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gsjqdkjse.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gnxfltqst.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gutaqubwr.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/grdckujhj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/ghngfqzsk.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/grkqlkrsl.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/ganoaedri.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gefyxpjfv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gkpngyqvs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gznejowaf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gmcvlrdek.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/glnsedhhk.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gcjbpfhin.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/ggjnkbuml.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gyeewwfih.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/glufdgrwr.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gdtbbelwo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gfifymkiy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gnczwctfb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gvqxohysv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gycxwgkkh.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gsmxtzlnw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gumxzxhjh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gfypnueaa.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gxvscznff.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gnnjnnhos.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gqmdxmwnw.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/ghzqqfihg.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/ggaduxyiw.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gpqoapdol.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gvndcfwce.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gxgilpuci.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/glntklcix.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gkxszrjtc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfftinazb.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/ghifdoekp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gndbcftrg.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/ghmchnkwe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/geipdfaly.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/ghqjdmlzv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gmfhkhyfb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/ggecmapfw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gatalxikz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gkvunenbw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gqcdigikf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gbwfwatpv.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/guwxgvide.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gzxayugzz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gikhfooaq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gwexjvwou.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gxzqxhgbr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/ggdavqmbv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gqedylsgw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gvepvlvxn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gbfacqmkw.sHtML

[H03] 主动抛出异常
来源：http://m.share.zdbjq.cn/Article/details/goefizrjk.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gqgccytcc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gqwowphgu.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gshchygxf.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/ggqhaomvy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gmswxbxbf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gopcyudzc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/ghdyfkntr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gpfipabom.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gjtbkczze.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gnkighimn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/guduptfxo.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gvwdrddlz.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gdgitdtgj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gsrgesyqn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gyncqntki.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gxndsxfub.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gufhrwmwp.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/grjghhory.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/geqixlton.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.zdbjq.cn/Article/details/gvnlknbkl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gwlvlzyvb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gytbadhpo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gukfbrujk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gchcrmjjq.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/gjpxpsfxi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gmqklnshn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gkdpojpwv.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gqhbblfjq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gyuoxkvrt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gtncqgfti.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gqbwakjlm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gbmlojwlk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gcaihftco.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gmxcptfpc.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.hesvh.cn/Article/details/gvswraeie.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gmubevuhj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gmkotmlrb.sHtML

PHP:  assert($x > 0);
来源：http://3g.zdbjq.cn/Article/details/gmhoiykcv.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gfujuxkhm.sHtML


<!-- 参考信息 -->