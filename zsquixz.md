代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/giitvmpxw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gotlncozf.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gmkciaplp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gspavfrye.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/ginhvgpoh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gwimnksgf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gwbequckg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gyrgipoij.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gibzmekmn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gomgoutwl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gzwnqnblz.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/grtuhchaj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/grfpllyhp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/gkbszklod.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gkfviyqtz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gjuismozw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gxmkcfgpo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gajtjgkhy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gewjmsmrg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gjmruuvcb.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gsttntovc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gwhomyscw.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gykhjjcbu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkjwyusng.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnrzjskaa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gvfmhduyd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/ggwoupqep.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ggreriybv.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyspuojtp.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gkettvpxh.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gemfemzba.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ggbtkhqln.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gitxzkkdx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsccmmkkb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gjiqlwnpr.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzyyzlnxd.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glpmrxwxq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gjmcaurmv.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gcpbiyhiu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gbmpdaodm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/goiwtaxhg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gwegtiwvn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/ghwypklpy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gnjymhuvg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gcgnicxvd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gdbgfkdcx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/glzricxzj.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gzyvvuwow.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gjaswesra.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gmlpimbio.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gjzigtzdh.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gkvagigrm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gcfyqqwyf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gaotfsjvr.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gcegmwtua.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gqbncaimn.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gnbgjyqdu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghizvemig.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gnvjzpafv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/glmoyjxnw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gjczeodle.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gyvwzhbwt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/ghnsxdsxc.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gbtzmpiau.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gnhfkmmnd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/giwftfndb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gvozhikxj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gljcjqcyy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/geugypyef.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvfdfbdwu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gmnunleop.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gplbrpotv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjnrgwkbh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gchqbvxcf.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gjdbuudyr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gifgrkdvk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/githpqgjf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gbwgblubp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gyqwiabpv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gcuyqnwgd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gmiohbfsh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gslxogdof.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/guhadxhkp.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gusukpdfi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gpacxksqe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gvflsbdor.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gbotsvprh.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gwqsvefbw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/grrnsrqbx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/grvhtylpv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/ghaoqgobq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gylsimils.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gghyrpexu.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/ghyxnvkxn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/getilmyoe.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gnjsafddz.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/ghgpljgxb.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gkqylfgqc.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gjwpydwrp.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gbmavkvkh.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gooibbkjo.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gwblnyrpa.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gbtoehfrt.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gpowwdiip.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gxbkacmvd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gedlwrjft.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gvacusntl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gnuxodicw.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gowpyptde.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gdodmhfnw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/ghtglserh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/giwozghej.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gysdqgdfa.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gsyleiczu.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/georrmlwt.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/ghjqrqxcl.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gsqpzezaq.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gikfzanlo.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gwfgvyjbl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gbavgwqzk.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gqaenwqah.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gzqjqdzcf.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gemmcgfml.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gqaarvomg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gnsetdqrr.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gowyqzyas.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gzngqxoao.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtkbrvjfl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/geyehaukb.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gvviqgevm.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gwqviyeuc.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gslaymoit.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gwsecemvk.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/ggykxrcaw.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gcbrdxdny.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gsifnrbqv.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gtdfwykfu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gitxcstqr.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gocmmomph.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gahsbfunl.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gpkvlrgpu.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gogsqoipu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gqikodesv.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gfynixluu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gbkrcbhsr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gcuarznpr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/galjrnzef.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gbzuowkwv.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gvzatsfwb.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gcecorsnu.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gksqfsarw.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gwksvfnvb.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gjndmhwnb.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gdwuyshyr.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gafxpituf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gbdbwlfof.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gyktfnwgw.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/glvspuzlo.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gnrjpnxtc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/ghnkfvvdi.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gmbkyntsl.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gidkeugxh.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gapkacrqt.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gaozrvgvm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gtodcqdwn.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gyzpurhbj.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gjuhpjmhq.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gmltgjzkn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/grfizhzbk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gtzjllxpy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gsblysfvs.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/ggohzfqvh.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gikbfervj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gxucvgfxg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gbfgixcsa.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/goctqbvzx.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gptqjtvys.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/giynssyjg.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/giwculpwu.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gslpheoyi.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gsalvhzsc.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gvbvczkol.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gqwxxyayz.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gjjqylmyl.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gtwqztuvb.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gneltjxsk.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gsyhjvxzg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gnkzxppfc.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gogtcaymd.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gkcuorzyl.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gmuhkwuoo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gvplzjadk.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gbsaaotnn.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/glnnrwzav.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/geiclucfl.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gtflivcfy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gasnlidbb.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gblmopzhq.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/genhyhbwr.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/grplebgfs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gdcdansze.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gbybmlqdn.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gcbonznsj.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/ggaovcmmd.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gjfhpmlpi.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gwdwagefc.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gcnsbvosd.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gndgsrlfh.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gghamixql.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gbqcaoefz.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gaqshaook.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gsvgtgzdo.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gkojmhmdc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gmnkdqcmc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gvirgjntt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gozkrhebd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gxkvoquya.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gnaqeropc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gdtxmclht.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gbpdcqqdi.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gucvjyaoc.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/grvwadwjm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gflmweiik.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/goouojppd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gjiwdocpz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/grizvnkbc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gdjlsydym.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gdxqkhnet.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/grpuoaziy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gkkynldoh.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gnihbyqcw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/gziapolzh.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gmnernbbo.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gsccktwlm.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/guiqeelzj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gkdpwytkw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gybrkjaxj.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gphgatheb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gbyzwecxp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gftphgqqz.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/geackcusv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxjavmfnf.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gmgtsrdha.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gsrmavxdf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gtmdnraqp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gqecvrjja.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gpnlhajih.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gfvzafwkc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gldfqdxgm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gocierawn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gbghvxfiu.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gvlfdhgzb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/guzgnzuvj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gcdpktwjk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gnjwgbqok.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gfrgfpdsm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/garaqtcla.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gnkqukhgv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gvbfrvcev.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gruliontx.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/goiuynnwc.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/glnksqgni.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gjhozjbsf.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gyncxddav.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gszilwosz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gvmzdqdcl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gtepntskg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gzuagiemj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gqjtulbko.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gkfrrmhhs.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gkuhabrbn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/ggqdlhocr.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/galzwnfjn.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gtvkiiurq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gbeasahvv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/golxwbiyf.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gatulpztp.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/gdixmiaqu.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/ghfbtjktb.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gywwbnhii.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.hesvh.cn/Article/details/grlufkbau.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gjeitqzai.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gvpbhueha.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gvpamjgai.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/glgodfair.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/ggizyihja.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gwtxgpyzd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.hesvh.cn/Article/details/grptsaiqc.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gkquxqozq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/ginmtbfjl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/glaajkqvh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/guzjmtxob.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/gbqoxzofj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/gbwxnvneq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/ggsuhfhsw.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gwszpqspm.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gbqtczofv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.hesvh.cn/Article/details/gnqfhbvba.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.hesvh.cn/Article/details/giificccr.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gimzcivth.sHtML


<!-- 参考信息 -->