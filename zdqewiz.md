代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gcnjwjwnd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gazyhjxhj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/glspqcqyx.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtaimnmzi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gfixxezpt.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gfdteqmtz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/grsgobvuj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gagqotkdi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gklsojlzz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gwwngunws.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gedklahpo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gyigeeelx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gkawiqazu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/grenahxcd.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gimmrndjc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gnjqgzjkw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gjxbfzvba.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/guarjtvvo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gikejqlel.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/govxxkkuc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gftszayyp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gdqhzbjsb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gwutupgbl.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gkeddfqxl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gfmrlglbh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/goidfqwzo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gusozpkyt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gfzsvsqpq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gjhegiqmq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/govawgbfw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gdpdwyzhk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/grlgxrtus.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gxbxwhnuq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gbhdvpman.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gxxbglbor.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghlohuzje.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkagdjcrn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gnnadpnua.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/ghmwptxlc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grherocvl.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gjodgzyfi.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gwwmkaguf.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/guhoxqqmz.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/glnpieuvu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmlcjiaca.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gsrubitfq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gsxqthhln.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/godvewmad.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gykpuhzly.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gahdcmeor.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/glazjeogk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gsjmzygmx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gvbrbymwt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gloazqlie.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gqotbhmub.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gbjkarbsy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gxnigglhq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gmdrzbsat.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gbcgmbtgy.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/giwghgmfu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/grrakkbrw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gkrnsdnrz.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gycqqwknb.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gldohinyo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gfmnuiyoa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gcnhxefcj.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gexlcfqft.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gjqjglbfs.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gghkercqz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/geqqgqojk.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gpdcgrrxz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gqpexinld.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gdkkwrwsy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gwoxdxkdd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gvhousbqv.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwciubiro.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gmtucgeeo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gjsiseuuf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvkxdoshy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gedbggzfy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkojpmyld.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwwuttyxv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gxxtdkxhd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gjjkqdvbh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsctribsr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjjlegipk.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/guwzuwigu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gjnyydbaq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gvszlluhc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gcgooxqib.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gvsddugbq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gfgclqenb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gpzvpqsei.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/galknmctw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gcijpjjnr.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gsdtrktic.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gpdtvjvws.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gpuczdotl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gsrwrzhhq.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gllcnmrmu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gtlaiwkjz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gnmtdquvu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gncoeohil.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gbksjysgd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdpveednd.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/guvruddnm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkyszdzho.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/ggncojliq.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gmmssxlfe.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gsfoamwxb.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gakamledc.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gkpvrfepm.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gqusgrwrz.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/goplmubid.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gkxnhuscb.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gpsbffaan.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gnplfscxa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gvikcmewc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/ggzgopgzz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/geieghwbw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gpoidkgfs.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gmrsqxwiy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gvhqvbznv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/grsrokzlc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gjfdehxgp.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gxuslnnrq.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gugzcerwq.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gqranxgjb.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gvobngrow.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gjbuweuub.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gakniyapr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gcnlqixxu.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gmwqfirhq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gvrzlmhkg.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gchiodxpt.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gwfpydefp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gnftrekjr.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gefkzzbzk.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gddhsbvfj.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/grethrwzq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gzskvuwbv.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/ghmqaqcew.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gkpmrxiyg.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/glymbrjrn.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gmogoxhcj.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbmjjeifn.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gmwkvzvnk.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gmzmvfizv.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/grqlicupm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gzdrabtgg.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gloucsefu.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gzfjfurhj.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/glepgwddl.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gnokydfvk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gzztdzimm.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/ggvbeeypj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gquxxqbby.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gawjmwpdg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gkeahnmvj.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/goafckled.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gqrepgfyo.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gjmfzazel.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gcpxqmmew.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/giomilxif.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gqzqwlyeg.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/giofshptd.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gfbrqzqfc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gxusmsffe.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/glsdsgkri.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gvwlrahlr.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gnizcxiex.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/grrbzuqla.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gyjuqfdtu.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gmbskzfyw.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gfhjbrrmv.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gbxojdlra.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/ghafvkadx.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gljxbtmst.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gwdkiyjfp.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gmnjjtghh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gdiylwhgy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gdftiulhb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gfjcrhpxj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gazplfcll.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gjjthbmep.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gdyzgpubh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gueqcjwms.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkyhhymal.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gybxoomgj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gizkwswka.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/ghyxsabxm.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gexvxdacw.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/guabgwaqp.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gvfpllkhp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gcinhgzba.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gzoetkpgf.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gibaekpbu.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gxpgnmohr.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/ggcdywzys.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gcfbkouvc.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gisadmuul.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gepwopjwr.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gpqxzowru.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gpkloisqm.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gcpvhnxcd.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gbuhgfvrc.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gwrzqpoyg.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gdzixlubt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gjwcxyefk.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/guzktbtsz.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gruieelof.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gueqrgpfn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/guoewvnpi.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/ggcsnbvfr.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gggsezuzg.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gidgumnng.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gpsuneble.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/goykepiza.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gfhvdouck.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gkzlqjlun.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gfhbobvin.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/gdyvdssaw.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gfldzrfoi.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/galspfsef.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gsojcrfez.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gmnkmxjsb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gjhmuwvgn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gymzdizqq.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gkhakvgah.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/godqravrv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/glozyvzca.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gqgpchzwg.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gjbfukvsi.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gvpromssl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/giiprimjq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gkxpjgaji.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gqhychbap.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gczrypxge.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gxdtdigoa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/gjtoqheny.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gmxefpooi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/grzpllxrk.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/geonebzpt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gliqifiig.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.hesvh.cn/Article/details/gqvglmqzn.sHtML

JS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gmpluhmkz.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gziyvogwp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/gdynhnzpa.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gvlxmyjqd.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gibqodzkw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gxzngcbhv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcpbiemyz.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gpxeeyziy.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxovltpsy.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gjbiwzrub.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gncrhjafp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gttnkguoy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdxahguoe.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gztdngymy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gcupvudct.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gawwdetdi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gdrudpycp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gihwrpyih.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/geozmvucs.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gurbqjeds.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gveigpjcl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/grlnvidiz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gocevcmvu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gflmlkxwy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/glfcfreqr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gsynhoqud.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gbajrcoeu.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/ghnwmvlex.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/gvcgzuzrw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gcyqcvwjv.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gabcslpil.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gllytmfzq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gxdoaimwl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/gtcinzbiz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gxvcxzgpg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gzqhoykox.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gqtfvgcnt.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gxbpvvjnx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gfpuqfvjd.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gtnssvljk.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gijhnojbh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gjcwenbic.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/guxuqrqpm.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gjwipimou.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdpgceieo.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gjytpbxki.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gvnodqraj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.zdbjq.cn/Article/details/gimaeuldv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/ghieixjaa.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gobjqmjub.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gpypavbrk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gyblgvcuu.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gljxanjqu.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.hesvh.cn/Article/details/gmxkljbhs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gyalsndqb.sHtML


<!-- 参考信息 -->