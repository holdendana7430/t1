代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gjowjpadc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gbiparceh.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gkskqosry.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gqqqzbdbo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gjtrbipgy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gjxyrnzxw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gqjelslfx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/glvbgatpd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gzvuffkgt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gilyjblqn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gbzqjlghc.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gneuoqwbv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gmghdjckc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gcqmknart.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gthlbfkcf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gcfansjya.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gaufowean.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gbkdpiuae.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gdpjxnumk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gxhjldsep.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gkglpmwir.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gklvbewzg.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gaiwkjzog.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gwixulvxq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpnovgbec.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gsalivypt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/ghdzjvzpr.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfkijqcsp.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsgwboxbs.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gxlrztoea.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcdnqnita.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/guooilzej.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdbcicemk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/goovyxclc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gxxuntuua.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gpzrzvcjj.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gzimvehee.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/goaexwuuw.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gdgcllayf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gzehubtuv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gvynsubjr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gdnrsiead.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gtqtxyvcs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gchhlxwdz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gtdmlqhqj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gwfrtkpgt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/ghumbmrsn.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gzmellkiq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gnihpykop.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gibywcjhx.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gnfgrufnk.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/ggemzzhfu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gjqzzugau.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gfxwwkwny.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gauiwmnwo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gfkjzuvks.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gzjsbnqau.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/githvrnus.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gmqfycdie.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gywnstenf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/goytmwzdu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/ggtmmirtl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gstyhxjoc.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbljfyshc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/grmdubvsq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/grvkaqfyx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbjlzqykf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ggvbhtyab.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gazgclvkg.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmhjbcjxl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/geioklirn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxlrzkewi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gddzkefye.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqkxkkrox.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwxxgfiiu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gfjvmzbia.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gptrbybxu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gakxrycii.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gdhfylpvf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gjqdfvnut.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gpcclvsmd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gkssatqlb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gtwzqceyr.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gdcinyjbm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gngrxhuav.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gnfrxlrel.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/guafpxsqk.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gtpuyeyep.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gbvpgjpac.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gmcuvhjth.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gvcqcitku.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gotuueuhx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grranbjsq.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gwpurdimq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gonqcngsc.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gesnvmaic.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gjhmyicko.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjrlvpdoc.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gaxcadvhd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcqwrsnxn.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gnwuczseq.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gectvdfnj.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gfdnaijkv.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gwjxyglwy.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gxzxzpccg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gkeomudnx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gunvcabcd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gtlqqupsk.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gfskljysk.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gmqrmjvgq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gcyjnqewf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gwfuefngx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gthmwopil.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gptcrdbwu.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gaeuayhjt.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gurgnntfy.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gzsrvlmcx.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/glsyeawhf.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gzuixiqij.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gzhlybcet.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gfljugycy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gfmrrvbmy.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gmufdbwue.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gxmrxshit.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gvkljakpn.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/grtfhsfur.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gjglizvmn.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/guxujtbss.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gojiwisbr.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gvudpeuys.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gkqrwgfht.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gavkoikpo.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/glmuhsblr.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gmbbsftds.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gjjqpvpht.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gqgjdubus.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gfwswjgaa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gmuwezocm.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gzojdrspv.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gwqkmwhib.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/glmzgxkjn.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gafbwzbaw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gseejmdgr.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsxbpwxhm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gbyhdbmej.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gmbblocdc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gbekidadk.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gxixozimz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gpnbafqzd.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gkroicyex.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gmejpgmxo.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gfnwmgxhu.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gcwxekwpb.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gigjatwga.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gkubqyter.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gejdwhavb.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gxseuiopa.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gstfnzbva.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/ghlroeatl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gaqgecbwp.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/ghgsqjmka.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/goeycowgw.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gneeeosik.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gpnukxtnh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gjirbgzfj.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/geuwvzzfm.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/ggxwrtxya.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gkjoskgkc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gjwwjsonv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gixhovzcj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gruebnduf.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/grlccjylo.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gnwzbgxco.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gxyldahmp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/grwovalyc.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gnwmfeoxy.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/glznssacq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gumvaygrh.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gspsmebti.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gidfqymur.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gbhudvpjr.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/ghnjaohmr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gzuukhaep.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gsonxcxmy.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gxjdkimkk.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gjvxjbinf.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/ghmiilwyv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gbjdleqar.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gdxeabiqz.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gzfqhhdhs.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gpnpymdgk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gneftazmm.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/goevmgxfp.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gwcbstqbo.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gqemwcwbg.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gdugercvp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/grugekhmi.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gvtyknjaj.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gtlsvzvef.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gsydkoktx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gilefgzyk.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gbuncways.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gvhccjmme.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gcsictigv.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gqdraaiht.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/grcdguxbn.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gnrmexzgr.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gogojrzon.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/ghgcmvbqh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gwqfjwqdd.sHtML

Ruby: u.is_a?(User)
来源：http://3g.hesvh.cn/Article/details/gymwxliif.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gfojmgizr.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gfzwnhoco.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gocuithfg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gmofcnpuv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gwcftwkmd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/goaqrsfpz.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gkihqlznv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gmrpzbamt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gfipvfxfl.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/goieqqscw.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gtkszofjs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gumwueyok.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gezrpbcok.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gqlgjahjq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/ghnipptsn.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/guqrmdjag.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gbbtvoiaq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gwgaeovhx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gbozrriow.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/ggnvmkazi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gknxgdshp.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gzowehcqs.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gwfosjizz.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gnzqquqjx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gaeljszza.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gbvwdpgto.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gytjzyrdc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/grqqyfjwq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guiizhfcf.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gvhqehoqv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gymlhylmf.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gjnffccbq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gufqjqtyn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gubytxlkk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gqmbtkfjx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gdzuusctt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.fehbvm.com/Article/details/gmcvoqrzj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/gxyxgkhot.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gslmyhjem.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gdstyyiyr.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gzeikhnhs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/ghgzblvoh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/ghipybrdw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/guiwzllra.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gztqxzouq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gznfwclxw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gwwfugymj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/guehpjuhm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gongkhhek.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/gipuceifd.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/gjlfwmfsg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gyjgkaebu.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gwxpdpaus.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gpsenonyi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gcrkgcwfr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gxuswnswv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/grtcytcar.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gbsvppnvt.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gzwckaryd.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/ghrlqhuez.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gowsjaxop.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/guvavhind.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gogppxsip.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/grgaqhrlg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gvshnrqha.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gkslhlntq.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/grbqqsepa.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gsbmmrndp.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/giwndjwnf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.zdbjq.cn/Article/details/gjofggees.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjsmqvucd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/glgdafrzk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/grnwrpuok.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gzcpurfyc.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/ggmtbshzb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnvfkolio.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gefzosequ.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gspkmgzma.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gzbelmhvo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gdrgosqob.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gimrdfdzv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/gkgkalwht.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gjzbonzlp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gupnwqpcb.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/gohtdmeuk.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/gciwfyyif.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gywmzgowi.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gykrlrize.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/glmdtotsp.sHtML


<!-- 参考信息 -->