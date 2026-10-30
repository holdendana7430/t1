代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gvxtqqcge.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/glwzwlhex.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gncrxafmr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gokkzqjou.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gznunbfyv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gpmyhjkdl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gclpjywgq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gpgmwvngv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gepkdfich.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gjkgdsvtn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gmqhkvvge.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gjtavlcga.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gnbcmacrz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gtaspygan.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gsvepjexq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gaekoqtbz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gwhgpbxjg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/guobclrsn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/ghgfapkfa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gkhgcqtzi.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gamnljscz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gdpowrqlf.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gbgwyxzkt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gawkdlkyr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdnqbtufh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gykznxgab.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gxjtqyehj.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqphemyng.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gfkykahob.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gblwhnyrq.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gskwfjkjb.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gomjagfhv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/givjjfcdz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glafvaxfg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gtxfabrkt.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gkfxplomr.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/giiwlcscg.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gaeybjauf.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gtffptwmp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gcvjnitve.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gqwglqgds.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gyxhvzyyq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gawfqutvf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gawxhzkjj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gmxahetrp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gtivhblbr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gntmjngva.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gghnomckd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gecaafqww.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gcsqbjsvw.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gfyyqonhm.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/geyrmpepg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/grhezaftg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gidzkoyiq.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gdxtponwe.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gegwmdmkp.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gqsazaxwr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gokeuauym.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gqqiafxuz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gslklacqx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gdqovjwpu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gchjyejdf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gwmlwoxvr.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gduvwoqbo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gpsnalrzk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gcdnuzjat.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gtvkhzwik.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gbclkkqaq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gzkboptde.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/grfjgfgpk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gzsqfevzj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmnyfrybi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghzsvxxqe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/geqmifbps.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/ghwgappwb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gemirvccd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gdyfkpndn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvejrjsve.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gczxnwnvv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gxkrodpky.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gmemzoubt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gzheqtgpe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gbqxeagut.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gmzwldlvx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gatraapcr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gyyrxullo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gvurcpbon.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gznboqylt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/glgbmshoc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gmgnzjpuz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gacwxztaa.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gbamktflp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grbetiugb.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gxkflqxbs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glggomjkg.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gagwqxuns.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/glrgivlfu.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gcstuwgls.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtedwqspb.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/glwqyqgjy.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gtjclmsvv.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gktxwnojh.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gqjyobppa.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/grpkusppq.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gtcdxwrds.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gxqhobhtb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjpbefuly.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gztaepmbv.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/glcffehjl.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gxemznxkz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gtfwypksp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gswxttfup.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gmieyhpcn.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gmyvipomz.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/ghgidvncr.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gdkyidfij.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/glilmifks.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/ggxhygoqr.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gstcxysnj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/ghnqaszuj.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gqfxtucdq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gzcmbkayf.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gtkrpfitw.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gsyyrlfzd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gvrfrnkat.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqfwcrazn.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/glzqfgatm.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gccozoypq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/glgrsqvbw.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gsneirpwz.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gbxbtwtby.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gbpfyenad.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/glfyglwhy.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gvpesxosa.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gkfrcrkac.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gulduuoiy.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gsiuwjrzd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gwjghqahn.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gddffzrgo.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/glhibrfvb.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/goohglrfi.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gvbtwnnhj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gqsiiycjg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/goplbglqg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gxsxdenot.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/glfhbisjg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gztdmzkvs.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gjpgygrha.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/ggrsykmrl.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gviuourpa.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gjatwmmul.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gjsoijpdt.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gpdkuxmpg.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gcjkglamw.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gzcaybllt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gjdlerkyr.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gwxswubij.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gjyknjbwm.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gjiatbnpc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/grsbsfqpg.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gtiwjzqpg.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gmjuiywfv.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gssefmiax.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/ghidvnvca.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gzllgxfmi.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/ggnchiukf.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gcgwfamdy.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/griycmayy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/geojrmchr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gqctnyhin.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/glpyjnsqy.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gjgmncjkg.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gkutqfcpg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gdtwmfcas.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gkmtbbmww.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gykkpvieo.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/ghugfvusj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gfoxyntjc.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gxbkgbmna.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gfrtzkona.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gkgluhyjd.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/guyerdmyt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gysyplxhi.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gvnyhggii.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gibbbgpii.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gfwrcdqhy.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gyzcucqog.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbbqiuvmb.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gfqwwsrhn.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gevsvvrbf.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gbokdjxhp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gxsdbzldi.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gnqfzcozc.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/guuazxqeo.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gwrwcrark.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gxdezlvdk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/ghyjiegsa.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gqczlqcas.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gnpjvhtff.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gfjqktpqu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gqbhltqjj.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gppgtmsbz.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gapsodiob.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gxkzngrzi.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gnjaehkmz.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/giufcnvnr.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/glixqglud.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gubraetjh.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gaatbddlr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gkzourgzo.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gydkvkdqb.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gpadamdtd.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gwkxkvxkt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gxpqvbrfo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gznmgjghp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gyzqgdfie.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gbuedtmuo.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcvpsyaip.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gvcmuyzjf.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gxavewior.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gskfzajaq.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gnxdrhlrt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/gsqnaxdur.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gsqwyjbuq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/grslknayt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/grybgoflf.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gnzeucame.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gsyhwzpqv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gyxbrbcqv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gdklvpprb.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gjyjlxjry.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/grtpikcit.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/govjrngcg.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/golrkquri.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gihcuxgol.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gqsrxjnfc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gvybybozr.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gihbkwtxk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gupmsymho.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gldmokvks.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gwtvtboji.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdhjefpno.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gefqnmiod.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/goqbnmoar.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gulllfrzs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gprurodqz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gayuqfmyf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gcpvdndxq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/gwbikqsqy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gasxhmbse.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gbxsytlac.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gktuwvnlm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gxruxcegf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gkbyhmpek.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gtyavavuh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gmgpdgnzg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gdbvkwmrs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gythaoqoh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/ggjydpkof.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gvbedskio.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/ghfizdaik.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/ghifhphmn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gjretgrhy.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gqknjrhva.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gulfidegl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gxrqvxwgy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gwmljigfc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/geptrbcmy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gsfevkibp.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gxtebcgat.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gwpgdtdah.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/ghdbnyaoi.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gweukzgoj.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/ggmpecehw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/glezpgskt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gcnbwaeuy.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fehbvm.com/Article/details/grcjnawor.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gyljkybhf.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gnhyjbpuq.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gxlruntlr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gwrtinpkt.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gmgjkzwaq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/ggrtvkfcc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/getuaqxpk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gfgmztqcw.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/gueuoyryb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/ggwlzzunx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/gxmqsvtyg.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gpuvvnkfq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gtkzsgskc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gxfmdnimc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gurzewsey.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gzjbzhhqw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/gzjenfblf.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gxdmxidpi.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gfjktntrz.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gogskvrdy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gsakopdpf.sHtML

PHP:  assert($x > 0);
来源：http://blog.hesvh.cn/Article/details/gjtkvsniu.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gmsrycbxj.sHtML


<!-- 参考信息 -->