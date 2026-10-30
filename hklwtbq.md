代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkujbfuj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fanxiaobao.xyz/Article/details/gnpmkdwdz.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtbbjcrl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxuxahvgq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkdeovgv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gopcohrgp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gephbogss.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fanxiaobao.xyz/Article/details/grnzwzkvo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fanxiaobao.xyz/Article/details/ghyadxali.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtizowmzz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsgfazuy.sHtML

[F04] 追加写入文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjazmrja.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gbbqxaguy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fanxiaobao.xyz/Article/details/gmwykmhoy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fanxiaobao.xyz/Article/details/gtkzhmedm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqijueyhx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fanxiaobao.xyz/Article/details/gontimfzh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fanxiaobao.xyz/Article/details/gautpcodi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fanxiaobao.xyz/Article/details/gqpnbxuix.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fanxiaobao.xyz/Article/details/gwklhaiqi.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjnlmgjn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fanxiaobao.xyz/Article/details/ghwnspvkk.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gvoceiqfo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gepexgmeh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsicznju.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtuhsnvk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fanxiaobao.xyz/Article/details/gurshxcbs.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkkudknf.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gyjrxyanj.sHtML

[F06] 删除文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcscrhuwe.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfijzjebh.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaugsxsbp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gfpeumznk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpvloavv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/giyojpjmb.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqllrxaec.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmupbkxg.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbkqlbjs.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fanxiaobao.xyz/Article/details/giqksytgs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fanxiaobao.xyz/Article/details/guhuhupbt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxifyrni.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fanxiaobao.xyz/Article/details/gjchfmplm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzrkzvmf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghclgxohy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fanxiaobao.xyz/Article/details/goqlcsmdv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fanxiaobao.xyz/Article/details/gcamxrdlu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrfygtia.sHtML

[F08] 遍历目录
来源：http://read.share.fanxiaobao.xyz/Article/details/govczwaqy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajxoaqdy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcnvzlqp.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gfosbmmod.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkhwzoyf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhedzewk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guezfnobi.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gkqbrffli.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcppsnzu.sHtML

[F09] 获取文件大小
来源：http://read.share.fanxiaobao.xyz/Article/details/gyumfquce.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrdunubd.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxuujemi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnzmcrvld.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fanxiaobao.xyz/Article/details/gaxomscue.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/giylpapwd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeohvyzi.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvgvgupb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fanxiaobao.xyz/Article/details/gztmmwwrf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fanxiaobao.xyz/Article/details/gepnbmkzs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhiuugcg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrigwcdy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhtnekni.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gcuxtgzba.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fanxiaobao.xyz/Article/details/glwmylwqg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gbuwbybst.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdnqrpks.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/grboegsnu.sHtML

[F11] 复制与移动文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzlviyxuf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlswnzgz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gppihrjgo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gttrhnqgr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gffekgzdo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymguojus.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghrggojis.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gboglrecr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fanxiaobao.xyz/Article/details/gkouzjtnm.sHtML

[F12] CSV 读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gliirnomb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fanxiaobao.xyz/Article/details/gbflmhana.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fanxiaobao.xyz/Article/details/gbleqayly.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfnugjas.sHtML

TS:   // 同上
来源：http://wap.fanxiaobao.xyz/Article/details/gcvjbcmsj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fanxiaobao.xyz/Article/details/grtwvxdlf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwuqcayh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fanxiaobao.xyz/Article/details/gqjnsyyru.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhchaaep.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gnxkzyzlp.sHtML

G. 面向对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltbuetvs.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/goqouihwk.sHtML

[G01] 定义类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggemgeryj.sHtML

Py:   class User: pass
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctfbapuz.sHtML

PHP:  class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gbgdfruba.sHtML

JS:   class User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrfikiyv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fanxiaobao.xyz/Article/details/goxhaxsju.sHtML

Java: class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gbnwyfkpm.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsugfjhpa.sHtML

Ruby: class User; end
来源：http://baike.fanxiaobao.xyz/Article/details/gcfklbvqo.sHtML

C#:   class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjhrsjim.sHtML

[G02] 构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgcukdpc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fanxiaobao.xyz/Article/details/gksgiazdq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/goejxfnff.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gopvzivjz.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fanxiaobao.xyz/Article/details/ghjurwxop.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqnackjka.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fanxiaobao.xyz/Article/details/guubggdwl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdetqpkx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gicfymdly.sHtML

[G03] 实例属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjxxefpe.sHtML

Py:   self.name = "x"
来源：http://blog.fanxiaobao.xyz/Article/details/gytjmrujz.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/glxvycgph.sHtML

JS:   this.name = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/guwcgbmzd.sHtML

TS:   name: string = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjfzmfcp.sHtML

Java: private String name;
来源：http://3g.fanxiaobao.xyz/Article/details/gndycavza.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvayeokg.sHtML

Ruby: @name = "x"
来源：http://www.share.fanxiaobao.xyz/Article/details/gthitjipz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/gjefozhvv.sHtML

[G04] 定义方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzauohmw.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fanxiaobao.xyz/Article/details/gspnlyjdm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gklfgemdz.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guhqozypq.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grtwaktjo.sHtML

Java: String greet() { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkztugin.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsakvcjxz.sHtML

Ruby: def greet; @name; end
来源：http://wap.fanxiaobao.xyz/Article/details/gyeohmarm.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/gkhzbeltc.sHtML

[G05] 继承
来源：http://baike.fanxiaobao.xyz/Article/details/gzufzosva.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjswkblo.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllaiowhw.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbeyxyqd.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gkilpfubw.sHtML

Java: class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkuszrlg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fanxiaobao.xyz/Article/details/gabswmkca.sHtML

Ruby: class Admin < User; end
来源：http://blog.fanxiaobao.xyz/Article/details/gmzyatohd.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsoietfs.sHtML

[G06] 重写方法
来源：http://wap.fanxiaobao.xyz/Article/details/gzttkybfe.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fanxiaobao.xyz/Article/details/gydmnowwl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbivopkcg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdelqdukk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/guclyarvv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmaaywep.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbuqokur.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gyniuulpg.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcbxakfu.sHtML

[G07] 调用父类方法
来源：http://read.share.fanxiaobao.xyz/Article/details/gknexwpuq.sHtML

Py:   super().greet()
来源：http://www.share.fanxiaobao.xyz/Article/details/gxajpiyhp.sHtML

PHP:  parent::greet();
来源：http://wap.fanxiaobao.xyz/Article/details/gjsbevuwz.sHtML

JS:   super.greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gshlnmtfh.sHtML

TS:   super.greet();
来源：http://blog.fanxiaobao.xyz/Article/details/govtjyzzk.sHtML

Java: super.greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gorecpnnl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggibyhub.sHtML

Ruby: super
来源：http://baike.fanxiaobao.xyz/Article/details/gnohpfoby.sHtML

C#:   base.Greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gosrlxlrk.sHtML

[G08] 静态方法与属性
来源：http://m.share.fanxiaobao.xyz/Article/details/giorcezuu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoixnuin.sHtML

PHP:  public static function f() {}
来源：http://wap.fanxiaobao.xyz/Article/details/ggmwlcyos.sHtML

JS:   static f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gnryujoiz.sHtML

TS:   static f(): void {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwegghtaz.sHtML

Java: static void f() {}
来源：http://blog.fanxiaobao.xyz/Article/details/gmpmspktt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gepdkdkgf.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzobcfnhd.sHtML

C#:   public static void F() {}
来源：http://3g.fanxiaobao.xyz/Article/details/gikifhzeq.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxmbizok.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fanxiaobao.xyz/Article/details/gktnusepf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fanxiaobao.xyz/Article/details/gslwdunkh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guimzemgh.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkjrowtca.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsptfsfi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjujgjkc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnkjraas.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gemkkzzox.sHtML

[G10] 访问控制
来源：http://mobile.fanxiaobao.xyz/Article/details/grvchrowt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fanxiaobao.xyz/Article/details/gfviepofn.sHtML

PHP:  public / protected / private
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwdawgqe.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fanxiaobao.xyz/Article/details/gmbophqyv.sHtML

TS:   public / protected / private
来源：http://mobile.fanxiaobao.xyz/Article/details/gijhftuhn.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fanxiaobao.xyz/Article/details/gfuborfmx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fanxiaobao.xyz/Article/details/gzlqyzlcl.sHtML

Ruby: public / protected / private
来源：http://baike.fanxiaobao.xyz/Article/details/gonbbnvjx.sHtML

C#:   public / protected / private / internal
来源：http://baike.fanxiaobao.xyz/Article/details/glnxpwsaq.sHtML

[G11] getter / setter
来源：http://m.share.fanxiaobao.xyz/Article/details/gbokkxmzq.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fanxiaobao.xyz/Article/details/gxmnrsxkt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gamffkmlr.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbmtwzbm.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdeyezfj.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gakyanzay.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/gmlbhdyxt.sHtML

Ruby: attr_accessor :name
来源：http://wap.fanxiaobao.xyz/Article/details/gsbasyjhc.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjaykawld.sHtML

[G12] 对象转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizmlwtju.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fanxiaobao.xyz/Article/details/gfbyvupez.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmqhewspf.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwirmgag.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzcwoofuw.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gninqwaen.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gimshoksf.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fanxiaobao.xyz/Article/details/gnjciwyse.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fanxiaobao.xyz/Article/details/gypcldmbs.sHtML

[G13] 判断对象类型
来源：http://www.share.fanxiaobao.xyz/Article/details/gnflsgknz.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnbgvfokn.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypkscsbd.sHtML

JS:   u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gtxvikofd.sHtML

TS:   u instanceof User
来源：http://baike.fanxiaobao.xyz/Article/details/gqeiebnqt.sHtML

Java: u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/grskwiayl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjlsvfmh.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fanxiaobao.xyz/Article/details/gpatgtouz.sHtML

C#:   u is User
来源：http://wap.fanxiaobao.xyz/Article/details/gcgxlajng.sHtML

[G14] 数据类 / record
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwnswzda.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmfatwyu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlvhvcgr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fanxiaobao.xyz/Article/details/gzxniakxs.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fanxiaobao.xyz/Article/details/gmjyegpyl.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gwvqvmjdq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fanxiaobao.xyz/Article/details/ghfrnzzai.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggqfzefa.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmfakszdw.sHtML

[G15] 枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gdwbcqcxk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzhrhzut.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkaonoskh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqshwjmt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcokgqyy.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fanxiaobao.xyz/Article/details/gyfvamurn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fanxiaobao.xyz/Article/details/ggsmijnlz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fanxiaobao.xyz/Article/details/gbbxqwpij.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiqhrkrs.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fanxiaobao.xyz/Article/details/gltvtncpa.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fanxiaobao.xyz/Article/details/gtjztlltn.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fanxiaobao.xyz/Article/details/gemjkaubl.sHtML

JS:   Object.entries(obj)
来源：http://baike.fanxiaobao.xyz/Article/details/gkoctbmni.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaytiisuv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.fanxiaobao.xyz/Article/details/gkzawecoz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fanxiaobao.xyz/Article/details/gfueypcgq.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqttiyui.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fanxiaobao.xyz/Article/details/gkdcbqyxw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gissweqcb.sHtML

H. 异常与错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/ghdhxpsmv.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfegopizl.sHtML

[H01] try / catch 基础
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgmhylfu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjmoadcx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gqlgcvibs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmynzqcqx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqltoohs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fanxiaobao.xyz/Article/details/gftjafyey.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fanxiaobao.xyz/Article/details/graoninba.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gytgrjtwm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fanxiaobao.xyz/Article/details/gslqumkxd.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fanxiaobao.xyz/Article/details/gwkzlvukv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fanxiaobao.xyz/Article/details/grzgxbxdd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzkyehyx.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnpuroyz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnzcjijp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxhnuwfw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjjjglcr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fanxiaobao.xyz/Article/details/gcnfdaypj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gefhdrmbb.sHtML

[H03] 主动抛出异常
来源：http://3g.fanxiaobao.xyz/Article/details/gjdsxwsax.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdakuiry.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdumwsphf.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyedsyaq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxhbjhtj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhhmdcok.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhpwfkqs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsyuudqc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gorqbgfbg.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqsrrnay.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fanxiaobao.xyz/Article/details/gdoqqqbye.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fanxiaobao.xyz/Article/details/gredhttgu.sHtML

JS:   class MyError extends Error {}
来源：http://blog.fanxiaobao.xyz/Article/details/gmzztsynf.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gadeqjskz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fanxiaobao.xyz/Article/details/gsywqeioo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fanxiaobao.xyz/Article/details/gehwbpkzg.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fanxiaobao.xyz/Article/details/gkhfcdavy.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fanxiaobao.xyz/Article/details/guladzlqb.sHtML

[H05] 捕获特定类型
来源：http://baike.fanxiaobao.xyz/Article/details/gwdlralox.sHtML

Py:   except ValueError as e:
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrapibwy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fanxiaobao.xyz/Article/details/gewrsloon.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gpxtymogj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ghliptcly.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gjhsditmu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fanxiaobao.xyz/Article/details/gkhpmmbcn.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fanxiaobao.xyz/Article/details/gfgyvrsnh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueuxbpun.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fanxiaobao.xyz/Article/details/gjvrjykuz.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fanxiaobao.xyz/Article/details/gzejawqtx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fanxiaobao.xyz/Article/details/gyuaazhrj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxidoluqz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fanxiaobao.xyz/Article/details/grywpqcio.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzridhekx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gofzomxyp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fanxiaobao.xyz/Article/details/grnhmyhir.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdkcwlgyo.sHtML

[H07] 断言
来源：http://wap.fanxiaobao.xyz/Article/details/gnzqbnzkp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxanmlxvv.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzayjqvxd.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gdszstgxx.sHtML


<!-- 参考信息 -->