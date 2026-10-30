代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gragdwbdi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gmtvyytyh.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/glqzimlus.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gjmtfgzsx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/glkllmvto.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gmtqnlaoq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gfxszjehk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gxdvdbivd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gsvshpvrc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gabfpfwht.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gtsnspzbd.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gvftwezbr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gqxzgsyod.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gamjjnpsb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gvflntagz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gadhxevjt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gltttaaub.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gfrxdzthj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gwluytyqe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gkvxxndke.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gbdkwjgsm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gfcyhgivq.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gtushkhwp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmuexjbuu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvdadevam.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gqcqonxgn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gumxddior.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyfirqarj.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/govolrqqh.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/ggqfwabge.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfrijhhoy.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/greoctwpo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqaojjayc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gdvuqaeed.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gepifzvyi.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/geaygzxfz.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghwajhmkb.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gqyerxhgj.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gnezkirbd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/glgtjuhml.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/glrynsdhs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/glyauyyah.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gyaphlycp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gaajqefvq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gxqpaptjg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gnajiudac.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gncqpdshz.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gcdvgjdsy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gaiyqyvuu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gwwtshkip.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gvpowbgga.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gzcxkhnwh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gixpsnaal.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gpodfbycl.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gdfkjilhm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gkizdgcbv.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gbjihqfbf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfqrzcons.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gqxamljbq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gdulqqmuo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gvbshewrb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gsywxoiqy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/geolcetge.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gducivgje.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gxrzqvacp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/glvvyvvdr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/glodjwbgf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gcfkitywh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gybkfjqkm.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghxtrjcxv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gxbpydjeb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjapvoewn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gmuhtakzf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcmtmeztz.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gpwrwlmpc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gwnbqmfdr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gsetvfzba.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gobqukxzm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gujnexjml.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gzlmvnffl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/giddwqdvp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/ghpyynqqn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/glqxymbaj.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/giqckuyau.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gvzbegavo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gqzrdhghy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gbsoxzpov.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gtupscmjp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gtwlknmnh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gdhfcpyhs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gpnpepcyf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/ggmjgttza.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gudepfssj.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gnmboplkb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghfmqcrgn.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gabbztttz.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gzoxvllhv.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gfresmnxh.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gsijlxbts.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/ggfegston.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gncuqvvqy.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gvcifvdwh.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gvmksyvfz.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gazjzgbzi.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gqynyvhsv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gcdiuogzj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gefqzbepo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gqylnhvhp.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gtsfeqqmb.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gmslrewlk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/grldimbst.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gmiongktj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/glpddsekr.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gyozjmguf.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gaybbyflr.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gkwgsssii.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/geozepukj.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/glognnavx.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gerjviiwb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gkgyjejeg.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/grlutkuzt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gdwplrbhu.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gbozofumb.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/guzeyrudj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gwnfzyqjx.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/greammjok.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gedrokrsc.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gbpfoysxn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/guckwmyqx.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gjglynqku.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/govpsvegl.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gwdlfnptk.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gslgqlifs.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gmpxbmtlq.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gcjdvysqt.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gpimhgpvs.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/glizmvgxm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gbmqodztu.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gxxugtrml.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gwghkxilc.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gzsquxlgi.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gtsfqdlji.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gxwtrsfjg.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gfedsyvee.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gimpoykyi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfiiurrtt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gkqlgvuts.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/glohnqhou.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/ggjiqnail.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/grwlmcecm.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gpkarwold.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gmlinjmrn.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gvqqybmab.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gxppgaovv.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gpqocujyy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/ggrzyhnuy.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gghmfaxwl.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/ghxqjgbxk.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gwgckhert.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/ggsxvffrc.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/ggwbxhqhm.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/geucpunmp.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/ggegpgtqo.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gybdzquju.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gxyvzsoyu.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gehordkyu.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gyddcojge.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gvixcwizy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gasxfghog.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gzcyuzajm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/givauevtc.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/grvuqyfwk.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/geapwnadw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gnefzfplm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gueaarzqz.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gcmymbgho.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gnpyaiien.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/giylfdvuu.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/glqccprvi.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/galijzpzw.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gisqqxqoh.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gvssopshi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gnlsjpibd.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/golnzseiy.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gyacsltup.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/grrmglehq.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gicxfebix.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gqvjojaln.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gwhqslqvk.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbchtienq.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gftyyntiu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gayheedpm.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gnpyrfdhl.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gfycxaewd.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gadlvnphn.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/glyzzitbu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/girxaylpq.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/grlvkvqwx.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gxzubobsz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/giwofkdny.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gukumbkkj.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gyfbtbyfw.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/ghzvlltne.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gtqpgnjxv.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gmnhpqson.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gimeaqafy.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gekishtih.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gcfcietkp.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gpzwryadw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gbirriekq.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gbadoyihw.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/grsdrveek.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gufpbjoia.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gueiutyoa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gjvuqryyd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/gusbgcsxi.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gxdnfguxt.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gsimpkpzw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/glpkynmds.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gzmyqkxtj.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gvctjipyu.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gyzriqair.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gwoihwgin.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gtclugdsw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/ghvfgjxvi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/ghsajwipq.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gakcqqxie.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gggldiepf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gpdmvchwj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gmzexpkyq.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gkkabmisz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/grihpanzf.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gznxtijnc.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gxojubjmw.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gnegdngzm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gttbarfcz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gfkaqrtyv.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gpacvlhqh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/gozgturpt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghkwbpigy.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gujakqeuq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gldpfaryw.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gkrknaquc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.fehbvm.com/Article/details/gzoijjwdw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gfngtdysa.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/geqarcahh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/grhumfnen.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gbhoqiqck.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/grspuhgnr.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gnkgyavki.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/ggpurnlam.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gagnrlpsv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gmpdgtaan.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxsaybdqe.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gfiyxkrpe.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gegvurwlk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gvyqpjgcg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gobftwfen.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gpufcnzeo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/ghsmnfvhf.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/ggswhdjlm.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gptjafxrz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gtcrmrxiq.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gljekgphk.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gqtsxgzxe.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/ghdqoikra.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gcjinxlbn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/grpzhvxrf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gxmbqatiu.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gtluhijum.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gqhrkxoyg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/grbczajbt.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gnftfhuui.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gkkrdqizd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gsueqsorp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gtqxckkxj.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gnmrendeg.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gxymdzfim.sHtML

[H05] 捕获特定类型
来源：http://baike.fehbvm.com/Article/details/giokueklf.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gwgbtypmn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/gnidkkebl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gezcxxhqf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gidtcntbb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gxurnrlpk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gtllrcnmo.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gbdgqkepc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/ggbubrxci.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gmysqonoj.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/gaxdmlmga.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gfthvtwym.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/giqgqnyhq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gukjiwlde.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gaflopuav.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.zdbjq.cn/Article/details/gaiuoamkn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.hesvh.cn/Article/details/gatsspgjh.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gljwvpaam.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/gmblyoexh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gttlhtlam.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gobrttavy.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gtozultdd.sHtML


<!-- 参考信息 -->