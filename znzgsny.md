代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gedjajbqb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gseyihzej.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyefpgyf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fanxiaobao.xyz/Article/details/gkdzjstak.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fanxiaobao.xyz/Article/details/guprwhyfb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxscbgkj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gudqvqiva.sHtML

[F04] 追加写入文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gofakdwkb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fanxiaobao.xyz/Article/details/gojugbndm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fanxiaobao.xyz/Article/details/gctvzkcrx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvghgesoj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fanxiaobao.xyz/Article/details/gzdqukozd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fanxiaobao.xyz/Article/details/gjcfgzglu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/guvohgkku.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fanxiaobao.xyz/Article/details/gfalokkvk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fanxiaobao.xyz/Article/details/guuxoytrp.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gzdylrynn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fanxiaobao.xyz/Article/details/gszhjvkzg.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/glvqywbpw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpmsqvzy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkromkog.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/gmwhokrrf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmmegokw.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtewsanv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrcnlzvg.sHtML

[F06] 删除文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwkvooxem.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpajfovwl.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwhweycb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/geiiursze.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgkguytv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/ghxqehuww.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjccghmyh.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/glrkcrrqr.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/goifeopcf.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqnpwist.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbpvvfxl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/glmmkcznb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fanxiaobao.xyz/Article/details/gozypvzdc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fanxiaobao.xyz/Article/details/gkfpobrrz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuroomur.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fanxiaobao.xyz/Article/details/gdzbhmbdq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fanxiaobao.xyz/Article/details/guotrvrnr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fanxiaobao.xyz/Article/details/gpltpyovm.sHtML

[F08] 遍历目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbvyerpl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudxmzkud.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggzgopfqg.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gavrmdfzb.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpskmxer.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fanxiaobao.xyz/Article/details/gqdmddsfp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gviwwfrqk.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsrdwiqw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gyqjobqdd.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumkpecmv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwenpxkst.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gwfzzcpge.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fanxiaobao.xyz/Article/details/gdqqudhjf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fanxiaobao.xyz/Article/details/gjsbldmll.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/ghhtpqxzn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fanxiaobao.xyz/Article/details/glkmgkzns.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvficyvi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkhyglfo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fanxiaobao.xyz/Article/details/gngjpgfsi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrpyjuls.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gocqrglxx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gjshzrvhd.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gdelcmnqp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwewhuxim.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdnjzhhra.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gossmzero.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/griifqcjd.sHtML

[F11] 复制与移动文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyasultur.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjtjktdg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixswxddb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gojkggvrp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnjguljn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/gipiyoalj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fanxiaobao.xyz/Article/details/gmqxyaisn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkplgyzeu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzdzwbae.sHtML

[F12] CSV 读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmqojyeg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fanxiaobao.xyz/Article/details/gcymhfmqf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fanxiaobao.xyz/Article/details/goqszrkid.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fanxiaobao.xyz/Article/details/ghktfnsjq.sHtML

TS:   // 同上
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzmejhxq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fanxiaobao.xyz/Article/details/gctghjxcw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyewzpra.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjupkhgp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fanxiaobao.xyz/Article/details/gzzrrvirp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonubdzwr.sHtML

G. 面向对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gxppqfpmd.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ggunediqs.sHtML

[G01] 定义类
来源：http://baike.fanxiaobao.xyz/Article/details/gxghflfif.sHtML

Py:   class User: pass
来源：http://blog.fanxiaobao.xyz/Article/details/gpaqnbopr.sHtML

PHP:  class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqtrypzd.sHtML

JS:   class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdmuwpzp.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdzzspbgt.sHtML

Java: class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gbglzkurx.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fanxiaobao.xyz/Article/details/geufpihaf.sHtML

Ruby: class User; end
来源：http://3g.fanxiaobao.xyz/Article/details/gkumnytjz.sHtML

C#:   class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqjajeys.sHtML

[G02] 构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsissuuyg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fanxiaobao.xyz/Article/details/gkrglnjux.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gjvvpuflo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gakwmybcx.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fanxiaobao.xyz/Article/details/glgbtamjf.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwrcbihgz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsrrqgpr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjhmdkny.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpuwoboz.sHtML

[G03] 实例属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtaoiihk.sHtML

Py:   self.name = "x"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpappryem.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyhzyodi.sHtML

JS:   this.name = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/guhzxkmfp.sHtML

TS:   name: string = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsonkvoa.sHtML

Java: private String name;
来源：http://m.share.fanxiaobao.xyz/Article/details/glxutlvzo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmblzjcq.sHtML

Ruby: @name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdludtlgr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxyxpvrq.sHtML

[G04] 定义方法
来源：http://baike.fanxiaobao.xyz/Article/details/gaqdobrtg.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fanxiaobao.xyz/Article/details/gdoszrxfv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fanxiaobao.xyz/Article/details/giftmevil.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdqplvib.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gawnvsqbd.sHtML

Java: String greet() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwupeerrl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqtlolhn.sHtML

Ruby: def greet; @name; end
来源：http://blog.fanxiaobao.xyz/Article/details/guknieaxm.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/gcafbtmkz.sHtML

[G05] 继承
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyydtrxlq.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fanxiaobao.xyz/Article/details/gubtifugj.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapimrvgv.sHtML

JS:   class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gedfzfwlm.sHtML

TS:   class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gbzcakmyk.sHtML

Java: class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcwaqhzt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgipqiko.sHtML

Ruby: class Admin < User; end
来源：http://blog.fanxiaobao.xyz/Article/details/gbvvjahxj.sHtML

C#:   class Admin : User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gqahkhilh.sHtML

[G06] 重写方法
来源：http://baike.fanxiaobao.xyz/Article/details/gtrcwtynq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadacwiwm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtpwbyesd.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/grollmwtf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxbiqcyn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrjtwtpr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzyopurf.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fanxiaobao.xyz/Article/details/gkgsvdcay.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fanxiaobao.xyz/Article/details/gkufrftdg.sHtML

[G07] 调用父类方法
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjuheolm.sHtML

Py:   super().greet()
来源：http://wap.fanxiaobao.xyz/Article/details/gkfamuwir.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqynrkcm.sHtML

JS:   super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gssfkjysg.sHtML

TS:   super.greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrxezzeh.sHtML

Java: super.greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhorphgd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gywpwloly.sHtML

Ruby: super
来源：http://baike.fanxiaobao.xyz/Article/details/genqpeyft.sHtML

C#:   base.Greet();
来源：http://wap.fanxiaobao.xyz/Article/details/grpghklso.sHtML

[G08] 静态方法与属性
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvjggqmr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fanxiaobao.xyz/Article/details/gructqdap.sHtML

PHP:  public static function f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gmczymywo.sHtML

JS:   static f() {}
来源：http://3g.fanxiaobao.xyz/Article/details/gzpsmojzh.sHtML

TS:   static f(): void {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtqoqueq.sHtML

Java: static void f() {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjuwvaoag.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkjluyye.sHtML

Ruby: def self.f; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gicmqetrs.sHtML

C#:   public static void F() {}
来源：http://blog.fanxiaobao.xyz/Article/details/gabxpkmwh.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqhcjrdr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwmzphhz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fanxiaobao.xyz/Article/details/grhsbfxle.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvbvjnsn.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grkkapgce.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/goyjmhpxp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwizxrjm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fanxiaobao.xyz/Article/details/gyoqspvpy.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gcsmvorth.sHtML

[G10] 访问控制
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkvprsai.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fanxiaobao.xyz/Article/details/gcyywdwjt.sHtML

PHP:  public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gwqyltept.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fanxiaobao.xyz/Article/details/gwtrbruzn.sHtML

TS:   public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/guhkadhnw.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrnigted.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fanxiaobao.xyz/Article/details/gjgwnagpn.sHtML

Ruby: public / protected / private
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymxzlpku.sHtML

C#:   public / protected / private / internal
来源：http://wap.fanxiaobao.xyz/Article/details/groxiezaj.sHtML

[G11] getter / setter
来源：http://www.share.fanxiaobao.xyz/Article/details/gczqonwdy.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fanxiaobao.xyz/Article/details/gyfqvodtl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gqebvstaz.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyluhhhhh.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fanxiaobao.xyz/Article/details/guqxikczw.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gillsjtuj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fanxiaobao.xyz/Article/details/geuidevys.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxgajtja.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuxmcedy.sHtML

[G12] 对象转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gizhjjsnr.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgxvqypk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gandgjwfd.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwflykhlp.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtutnkecw.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/geefgzqsa.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fanxiaobao.xyz/Article/details/ggedggnbq.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fanxiaobao.xyz/Article/details/gxutikejz.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fanxiaobao.xyz/Article/details/glkybdpfk.sHtML

[G13] 判断对象类型
来源：http://blog.fanxiaobao.xyz/Article/details/gkmoynlur.sHtML

Py:   isinstance(u, User)
来源：http://blog.fanxiaobao.xyz/Article/details/gythmvusm.sHtML

PHP:  $u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvwelngd.sHtML

JS:   u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuirstdu.sHtML

TS:   u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjybqfozt.sHtML

Java: u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/gorplobfz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fanxiaobao.xyz/Article/details/gxvhwkjvx.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqdkyayw.sHtML

C#:   u is User
来源：http://blog.fanxiaobao.xyz/Article/details/gusmeofsp.sHtML

[G14] 数据类 / record
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzojkauy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fanxiaobao.xyz/Article/details/gujyfqugl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fanxiaobao.xyz/Article/details/gvzffszmc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjyjhqij.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fanxiaobao.xyz/Article/details/gwzwsqfid.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejeghljp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fanxiaobao.xyz/Article/details/gfdqoksni.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fanxiaobao.xyz/Article/details/gpoylfjve.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fanxiaobao.xyz/Article/details/gojctisma.sHtML

[G15] 枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gdvgduovc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gbyakzpqn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gddkbhugq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fanxiaobao.xyz/Article/details/gdozcvjva.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiykrdxr.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdwpnyvw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtncnbll.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpqowxsp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjkmcwny.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fanxiaobao.xyz/Article/details/glweqqqdh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fanxiaobao.xyz/Article/details/ggkamajzg.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpedukgb.sHtML

JS:   Object.entries(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gkocoxcam.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdslstbmd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfkoxslp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fanxiaobao.xyz/Article/details/gsgbngpbu.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfcjrbcy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fanxiaobao.xyz/Article/details/gnzqbpowj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxabzgnsz.sHtML

H. 异常与错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gbjswgkcv.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtdifzqc.sHtML

[H01] try / catch 基础
来源：http://baike.fanxiaobao.xyz/Article/details/gamyawkwl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fanxiaobao.xyz/Article/details/gqhqpogei.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrxjpfmz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gnkikhoik.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gnqgbojbh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fanxiaobao.xyz/Article/details/gintxhpvj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fanxiaobao.xyz/Article/details/gqytpaxrx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fanxiaobao.xyz/Article/details/grlgdpcof.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gocenkftg.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gxlprvyqa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fanxiaobao.xyz/Article/details/gcestgvcz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gbkxikdfo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzpvfnvu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gskyckach.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntsfiypx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giftbhslc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtbefhdh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gkwnpsmtd.sHtML

[H03] 主动抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhbioyzm.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fanxiaobao.xyz/Article/details/ggwenyfuf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/glwcgtadr.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gyiieuomd.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gohkmjvsm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fanxiaobao.xyz/Article/details/gvbqqvagz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fanxiaobao.xyz/Article/details/gcbxkpmbh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqozdtkyd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/ghycgaaxw.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkdmwkci.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fanxiaobao.xyz/Article/details/girwddgsn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwwjfucb.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxhinutm.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fanxiaobao.xyz/Article/details/gksarijzr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkjpfygx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fanxiaobao.xyz/Article/details/gpcsbvtkp.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gutvrgcjn.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtjfcvod.sHtML

[H05] 捕获特定类型
来源：http://3g.fanxiaobao.xyz/Article/details/gsrcekwoj.sHtML

Py:   except ValueError as e:
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsehmfnl.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajiyivuj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fanxiaobao.xyz/Article/details/ghxmepkra.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmtfssjm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbykbeqo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamtbhcln.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkjqekyr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gnlhlgyje.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdghhbott.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fanxiaobao.xyz/Article/details/gktlstkjj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fanxiaobao.xyz/Article/details/gejseuhkh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/grqxhgqbg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fanxiaobao.xyz/Article/details/gnllobriy.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fanxiaobao.xyz/Article/details/giakmzwli.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fanxiaobao.xyz/Article/details/gyeadgwkd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgkhxgjs.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbiwdpoh.sHtML

[H07] 断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gytealexx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkyeqozq.sHtML

PHP:  assert($x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gdszclvpl.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkiuydgj.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gifyofxzp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfoeybtly.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytbarsex.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbbwewap.sHtML


<!-- 参考信息 -->