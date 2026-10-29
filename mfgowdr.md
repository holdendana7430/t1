代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/golpieasa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gifswgoxj.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gmaqpxamd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/grvslbwmj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gwnuhwfnu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/grrokyvdj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gaqxxynvt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gjdsjfjwb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gvdoqngla.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gmcvzjuvh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gdfpsamsf.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/glpyrycbo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gsibxcyhq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/govlmowpq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gambizskj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gqnfeserg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/ggsyuewel.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gyfekzlkh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/grcetwaiy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gzrfhlshl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gjrddscqx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gwlrrcdyu.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/galloykwu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/givlgduev.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gptanfzxq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gqhkdyrhf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gwbxfhtio.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gpjklhgim.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gnetnoauc.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gvrhvdhnq.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsblyvela.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/ghfqwsmgg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gksvqlfts.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtgwirzem.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gugkzpwtx.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjsqvymyv.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gnwxptcxl.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gvbqsjebt.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gtpyvwxly.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gfmbioynd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gbjmjltow.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gpypivhkw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gmvxinlhz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gbtzlpnxn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gfbbhisdi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gqkuwkeiu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gayiinpko.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gaqnveuvm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gxpgatxih.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/ggtzbrsru.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gsdskfhqe.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gjxihmayj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gflxuzrqn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gfgjjupdu.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gowsiiphu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/ghmqblbiy.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gcoppwlqg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnoivjrwz.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gsfbqvdes.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gradebedb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gcourchzj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gtbizfgwq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gsvssxqnj.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcuoikjww.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/goikihnkt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gnbobnpto.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnlbvhnsb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gyfvbdgyc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gntlloenk.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/glaheuwup.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/ghawdkxrk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gcplvovga.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gvxeznfat.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gawlejhzn.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gzhjtvygy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/glnixlyhw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gxljifpdt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkfwyfamb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gyddnlnkm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/grtmvlawa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/glabhkjxb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gbqetdwsy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gaadcdsbf.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gowmgxxzx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gypmhmeob.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gwkrkmlgi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gegwtqbhx.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gbffuhsuj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gtshmspoe.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/ggvtzunwf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gukrgpgwu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gejpuuuyw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gftbmxemh.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gpctqrfkl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/guggvqpdd.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/ggehagvnm.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gnyaosqka.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gjjfnmuff.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gnpeultll.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gecmokqyb.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gvbigafrf.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gkjttjptw.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gndgbjyvl.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gghvwvlam.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gnzkmtblh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/grvjnzutx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gggemqtaf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/glalduvnq.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gqunatrfd.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/giehoolfb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gdmribyxb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gbyundkik.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gwnbrohrd.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gyhdgmvqy.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/guzjropcf.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gnkrwbmhl.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gvwqvksre.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/guuirkiyw.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/ggisijzoj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gmwcirlyf.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gcnpnnxei.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gkfiicjwb.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gjxxjqmsk.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/glwarnykz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzkmiilok.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gshozoodg.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gjygfxchl.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gzlpelqxx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/giipxfsoo.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gqudmolhe.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gincwwmex.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gecckrchp.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/girgvzkwk.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gppjghwwr.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gkucoyhed.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/glvwcdski.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gfpdpqucx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gzcuykywm.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gsuqhgypi.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gyeoajiyh.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gicwatmxs.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/grppvuhhm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gbudmlral.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gaibiphjl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/glgjvhkmj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gzohqgqys.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/guxdlvros.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/ghxgbdqaq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gjphabjia.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gcdoejexs.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gtzpwwopo.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gpwqlyraw.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gvjruiuxu.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gpnstmczt.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gxkreuzqx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/goxhaytji.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gkwtuekiw.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gujnamwin.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gnlnaxemd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gsgmbaldz.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gsqtallas.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gpzlbvqga.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gbcriizjl.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/geqoyjujk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gfzbqvzoa.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gbehckjhw.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnrdvshhc.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/geppwtqtn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gzlxycxsm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gfkxxjieh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gzrbfjxsu.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gzxwdwerc.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/guqnlmqlr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/ggnsdpopd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gcenzznvx.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gkemrcyvk.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gqplwquam.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gbvcimgah.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gkqefipww.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/ggfxnbmfq.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gkfwbvptx.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/ghgbetfyx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gqolqgzny.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gcdfitoos.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gweoffhvg.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/guueycrpf.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gyeennuze.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnarywtmt.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gjwxtvpqm.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/glvbxkoua.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gcpoduegr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gwpsxvnbh.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gpmzqzdnp.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/guwjflsfs.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gsqtdpmrw.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gthatyqag.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gvjaibakv.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gjgomvjan.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gqmmlhvvb.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gyhemcvga.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gyrwvzcln.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gvjqbkdbu.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/ggllnhtdl.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gjzuoqyqg.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gwcctytky.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gwojnhxjw.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gjsgsgdqt.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gfwhyaogc.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gzzgnkqio.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gaachowmt.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gconxknpo.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gwcibvidm.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gzykexpnp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gqobgybri.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gloilvmdk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gptkfpwvm.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gvnasawkl.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gpxzqnozd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gguetouag.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/giwwpuqdz.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gxjqzaykb.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gqhzbguoo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/gefyjkhwg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gajetcnby.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gshjtnllm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gjtpgyapi.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gjitnqysw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gzdzoskkg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/goifrreji.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/glxvawsqm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gnsdlfixz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gvepjffdh.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/glcamvqkf.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gjzxhilqk.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gflhxlrov.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gcjfjulwc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gbzbcqlmn.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gtbheoxju.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/ghwackuuc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdpdciuof.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gqbdusvwb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/guuqcrnjy.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gevumwlpj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gaswybwzs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/gyrtqlkml.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gsefpzuls.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gdrnxymmf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/gasmuayex.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/giyqozdzv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.fehbvm.com/Article/details/grmofihqh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gjqihdfqf.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gvzgjqola.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gntuwzgmr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/goekbvixo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gpfzjobxr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gyixkywqw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gtlxkaxgw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gcmkhyqff.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/glbyblzuv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/ggdyckzkr.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gpyiuqbbk.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/gnnixmjxl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/guatandzh.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gdghbswge.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/ghjgkrkmg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gttyujwgy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/gggjicivv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/gumozsyra.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/guiolrksa.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gdlobzlet.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/ghdsczjke.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/grpdpsefl.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gminijsgh.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gtjhmugbn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/galdnimjw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gfkzevcfw.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/ggvoszezr.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/guirldzhp.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gnfxxrngg.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/grmjsmjwy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gmqrstnql.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/ghtnsqdvj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gbzxyerfu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/gfwucehxo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/govmzrhzp.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gtrbjwpkv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/grmmntlea.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gtfksxvhf.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/goobfxavx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/ggtzeohzk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gfhscceqc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gyceyjafm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gzovmtcny.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gahljrglb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/geefpextx.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gormegjbu.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/gwlzrzjyc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gnmecsxbi.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/gtyxmqnia.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gsoclqnto.sHtML


<!-- 参考信息 -->