代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gjyoomyug.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gnjbvdarl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gfrjkrzhq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gxoxvytmb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/guwilttap.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/ggkqwkusz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gjrubgqev.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gvfvsxszh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gfezxuemm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gnhraysfo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gjyihbypo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/grnuqfqvn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gjfubsyho.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/glhjuxqjh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gcrvphyvw.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gzilpnxrh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/ggbxdejzo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gypdgnyrm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gytvvqcbv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gthnsbeym.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gntlfllcp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gzkcyeqqv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/guktwfilv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/grcvoxlpk.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gkwktkzlb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gbxclgtyn.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gyipxssbh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/glntvwpju.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gynrgnbvi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gzqoasxth.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gizyxyslz.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxmuxrncz.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gubssezep.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/ganisesmn.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/ghmrosyxe.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gcepeuizq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gcjflmezc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gidkcgqch.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gvekwafau.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gpzcyrvzh.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/grihgtznq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gluorvboq.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gbrvjeufl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gewvvymay.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gzhwivmpa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gtywcsfps.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gvbqvwmyv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gnaxejtuo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gzmssyllz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gkoyqpblm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gieqtzkdn.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gmetkolud.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gpipmiqwh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gppohpijr.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gyvjbzryg.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/grxkspokl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gnmjfalyw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gzpcnuxub.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gwvgfllvx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gxpmdymth.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gmmnmoslk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gucszdnpy.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ghwwmeaui.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/ghsaplppu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/ganrprxfo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/ghuukemjn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gscnwghfu.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkzyvptfu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gofzyermt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gppwyubul.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfkbxcxvr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gwepbzmfb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/glhevonzd.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grotbomty.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gnqywjubc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gbmzxqgdl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gffimxvic.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/guoztijmk.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gzjqdcdlc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqhioxuix.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gjywjyjqc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gpvjifubb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gfbkjlvoc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gwhuqwgfm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gxvfpahqq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gvfysvxbr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gjhavpiuw.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gcimeebvz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gpmajiebz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gvwngcsoi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gkiqcxlnu.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gzegkceqw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gjwgycyza.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gjvisxqkh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gyodltkno.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gfllfbaqm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gccyxfhqb.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gseyrkwnb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtpsjwcnp.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gwebkluco.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gtrjtbawh.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gnakuddqe.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gzqarvobc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gddhjarah.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gwjozislo.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/guqwkxnjm.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gczgklekh.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gwiyvbanl.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/ggidijuaa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gtoavmzie.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gbvpuurfa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gctckfjxg.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/glvjeijae.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gfltvuwmu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gcsbskfnx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/grxysomsy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gsztshelb.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gawtugjhi.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gsxabmbsk.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gdejkaqaw.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gwglitwaz.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/ghbdohalt.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gnwxmtyuu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gwpbugnrd.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gdfrmdlan.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gedaahafp.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gfxjhbyij.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gwxxwmfzv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gosduiqkz.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gqzdtrati.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/goykjqkye.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/genybcjxu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/grzsqaumi.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gcojefmpo.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/grfiuqqhx.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gpwqowzdb.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gunszmdtu.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gmmydjrym.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gnmfxbsjl.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gbplcvtrf.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gqzuuoinq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gzbfiamxg.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gvzgcvexa.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gowlreqhs.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gfghytbum.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gerzgdppf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gobtpyygq.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/ghhjkmjzt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gejcovvmg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gghmcatzi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gisbigmnt.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gaxrcaidf.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gavmmnofq.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gihosdrpi.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gixndylxc.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/ggldnocnz.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gnbvkucwg.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gdoernavc.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gjphpxtji.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gizwecgfs.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gytrqxwhm.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/glxvnlowr.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gkmawwsoi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/guqrcrlmr.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gtntcfjbd.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/grzlcwkra.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gjumyunmm.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gcsiijgkl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gzwvfukqm.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gxbhiyciw.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gpvggwszw.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gcrxzqauu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/grajcdgvm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gdzjhppmd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gumxhrojx.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gdevmwqaw.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gqscqmvql.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gwdrzxuxm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gmhsmovdf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/genabtive.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gjyovbywp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gvrwuqatu.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gkjgrarhp.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gweyovshw.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gsysdkbtt.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gtdxahhrv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/goskytere.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gqtrujzdt.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gooekdonp.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gbfnqgugy.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/gexoxshla.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gpoxmkmvt.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gqguiaqer.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghcimfgbv.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gsumcdkxi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gwsabxgyn.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gxbfhprnk.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggwtidruk.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gghavlpjb.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gfnxghquo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/girqvaopj.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkdvbqruo.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gjvcykfah.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gcsjasbea.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gtposckrv.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gcxwodiet.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/glqqnbysc.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gmqxbwccl.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gdydvgnsj.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gchdylmoe.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gicgeiiyq.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gbisfubjn.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gwzqcsgct.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gypwemupb.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/grlzaxreq.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gbpqlpiad.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gkxcbdyzq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gmezkxvat.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/grbjsyosd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gjznulknf.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gvvteaseb.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gufxzxeld.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gdfjfodkk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gzkecwtzk.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gwmflleiy.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gbxepkidg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gofuqsxov.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gentbsuix.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gyxsspsdu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gfkggcwoj.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/glfydwloc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gnhelhwer.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gjwvkcknr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gylwigsrq.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gwpcbymim.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gjicweiiw.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gojfuujgs.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gdrfmpnmb.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/grrfrlwth.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gnjcazrmy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gspmpocho.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/gencjyxib.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gwwkwrxod.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbpzdfmhi.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gwnxxsieb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxhqipvqz.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gjwzvhjpw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gurvtanyo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gzgweguvg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gdceetbpl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gztwaukhb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gagohaizo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gcyiowqqo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gpgmxkbun.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gkyymhcpg.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gqenmjctq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/ggvyvvngd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/grsyczuzr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gprgzkvgj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gtjyceplk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gxifrpbph.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gvajcjvic.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gdkgmdtxq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/ghvohxfdu.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gbgzwxadt.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/gcstzbppf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/ghkawrpev.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gxotvhgoe.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/ggsjghpqp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gbzoedttf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gvvlqawil.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/grgdglhwm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gczrbyqzo.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/gbjsgixic.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gweiygwoh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gwnxyybgd.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmmzcxjfm.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/ghzfoqckg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gqvhwcpxo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gvshvnuys.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/gohmymqya.sHtML

C#:   class MyException : Exception {}
来源：http://baike.fehbvm.com/Article/details/ghuxbfobc.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gthvjyukx.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/gekoniwzz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/gjomzvjfy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gdvkoimhe.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvyxnytmv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gcfudfgav.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/gezchqyko.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/gwnbuvncc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gobpbbjxl.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gvsmsvskp.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gsohoschw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.hesvh.cn/Article/details/grguwhtza.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gxgqzpcwe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gzjjizbni.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gbvguyvph.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/gebcpgfsy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fehbvm.com/Article/details/ggphrbcub.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gubeppubv.sHtML


<!-- 参考信息 -->