代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gzzvctkwm.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gpagvwfjd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gwfzlomfg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gnpklzxaz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/geigwdlxp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gcnvevnks.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/guhwwsyar.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/ghjfioyfp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gpctlvenv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gfaawsciz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/gfqdikjkl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gludczrwa.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gqxcrwzoh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/grxyqopgu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gojagehoc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/grulslfqv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gokaxdnzn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gbxdirvxc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gmcfwqlrx.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gjampwtja.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/guqfeetww.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/glcaaqbqp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gzvoqynrb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gistubxyu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gympuedgf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/goyanasrg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gbvpozjob.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gbunduknq.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gqgrtceym.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gzijkavkd.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gihycnsvk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gcnmhwbna.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsmlbuyxp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gxrygfddj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gwoemxlbd.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnspjfezs.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkalwsjgv.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gajhzjaeh.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gckchctri.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gbvsiivqe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/grtrirgus.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqlrzyjyb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/glqcuspqp.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtlndzgzz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvziscwbh.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gbtvammiu.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gvgdsebtq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gietdwicb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gkkjlwxtj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gjyyedqxd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gqvwgykjn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gxhjvpgar.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gsghyxdsk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gijjjmxhn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gycvyetab.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/grkncortn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gkdlpraeh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gsxfntbhc.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gswhirxrf.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gpxqfgvfn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gdzeplqea.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gqghllxxr.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/ggayzespx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gvekdtsav.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gtuudzids.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gkguzdzko.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/grrnldrmn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/ghbybucdw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gxdkdbnuq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gefciriep.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/gweheujen.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvubxxswd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gneizhikl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gedxtfrlz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gerjimtgb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gapjfwgcs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gygidrnhg.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gluwgiseq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/ghwyhmjzg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gkmohacjl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtujdhzok.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/grdzgxppp.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gkdbpochy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gixyxsowy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gemfwrmkh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gsqfofdcj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmtzipmdp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gtfvadeez.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gskglmvxs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gjizkfqoq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gfusnktbf.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gvcvdpbwt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/glaffvfjv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/glpxwlgkt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gqbkvrjqh.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gjujpwnmi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gybpzppor.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gdwpumvuo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gxhtbrtnj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gjbujojtj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gukjkqbiq.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gdkkrdzpv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzhjgebtw.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gyuemmmvh.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/giuhcojzv.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gtbygwkgl.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gfteahykq.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gmcmnmjgu.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gcytrcqpg.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gawgnydfd.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gpkjdcsbm.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gxtwjmnlr.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gzbhvjied.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gtulzbcoi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gcirhctbu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gzzfrdpms.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/grejhjveq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gpbjceywt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gmoozuzkl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/ggxmrmuua.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/glorbatgs.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gwfphbpys.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gddqghajg.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gunkmmmyx.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gxdunysfx.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/ghaqguxmq.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/githksnhh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gdzesknkr.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gurqotohh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gmcbilnkg.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gfffwjwqh.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/giwsqzqry.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gqwqbpche.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/givanblup.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gkkcgopyc.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gfnfodplg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gcuswgxkz.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gryqpsyai.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gaospfeeu.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gnnnbojuv.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gclmanxrc.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqlkeakes.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gqsatldld.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gtmszprlr.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gztcvgytx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gwrtojdez.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gjouvhvux.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/ggnpqjmnn.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gqdefjvzv.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/garqwdejp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gnrwojnsx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gyjbwuwbm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gueidsral.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghmmkgarq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gokomlwlc.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gwnnoaxwq.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gayxzikob.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gocpikuin.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gnovluzdx.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gpwwzrigz.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gvfcuslmd.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gzahmeifj.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/giugexlxe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/guxhbclfe.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gqmegbgjz.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gmhjghyqh.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gndxsaczm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/ggejkmrcg.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/geiuglebl.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gnhyswuoa.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gqwhkxjzj.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gfjmgrrvi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gmcqcssxp.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/grrpdsriu.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/ggwdeaxgx.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gigxgvlzq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gqsvggdsn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/guiazeqss.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gdfikcvjd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/glmkpjbac.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gwephhaxi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/guptrbxnq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gtlezktuq.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gpptzpfhj.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gkxmvcnby.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gmmjudvbl.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/glcrayotj.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gjfmjtwnd.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/ghbgwcmro.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gubjdklmg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gxnoeziud.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gorpznhtq.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gjjpmzafl.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/ghrsrkgwx.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gjcqftscy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gvryuqexw.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gepwpnjmq.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gymysncac.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gwplaowvm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gtoalyqet.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/glxahrjqs.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gtzyvyndz.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gxwskzeta.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gkfplkemx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gviqbrwio.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gmrtgjnqc.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/grgkppfer.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/guyxxznsq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gtkugdtob.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/geimovhsf.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gqqujogiz.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/ghltvrvgh.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gxqawtint.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gonccionp.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gwqfaylhq.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gtqdqcukw.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gdazvisfd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/ghfskmsuc.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gclnmjwaj.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gsrvrcfyi.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gricayogj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gxvnnmdyu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gqxweimfj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gtjzalsfk.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gnojvwaza.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gflwnxgdh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gpunehege.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gitjvtoed.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gueopvzoy.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gomvcpfve.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gcrdyazwh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gaqmvdmpt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gvvpnsedv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/guvmoanog.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gbzrmudbx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gtjaxktyn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gxtrmrkgz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gpkvwvuck.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gezrjexsi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/ghpbmylrw.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gagqdjysf.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gwwglbnqo.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gpmvrhrke.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gcumpmupg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gqyduwepc.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/ghhkmoufa.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gsnahdsdi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpzkwqivx.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gaqchbewt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkihtgpsz.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gxnlwmgbo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gryxfxnpy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grlvdhhwn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gbnnqczeq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gmkqomtly.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gfjdpzlmo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gcufnxmxi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/ghpngnmpk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gbznxjklf.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gmosxfxfa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/gvvuoeuej.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gmhnzvdkl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gqnkqtydi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/griwspqve.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gjzoiqlat.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gkiqdprun.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gdsktgucv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gffqyddin.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/gvewanucp.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gtedkeoxv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gbvnpydqf.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gcohezpzm.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gqayftvlg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gspddursz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gyuzkwsmy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gddtijwko.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gmljqnpws.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gbsrkkqzo.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gqziureet.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gpimcelgg.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gvvljnanw.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gywudeyub.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/glhluvkxs.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gytuwiqho.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gjkqsuhfe.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gvvkhtefx.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/gujcvtoms.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gisynabex.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/goimkdrds.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/giqihuzii.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gbujhmhhs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/gggshuktp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gznwcgkjy.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.fehbvm.com/Article/details/gsfcodcxq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gnqgegxjb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gpjdkegbv.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gyhnlpotd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/geavxhpsa.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gusylquvd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gemmqifaj.sHtML


<!-- 参考信息 -->