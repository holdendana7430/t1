代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gwrqzoscu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/ganhixvdv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gaaksogdi.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqzxhmmdn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gaeshbqbv.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/ghotbhvjm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gotackxzt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gbzhyzymo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/goupbqxjc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gfkqimjql.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gqpqktran.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gnkuzvicg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/ginpifhfr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqcvktesc.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gqvtisgrr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gosbltmrk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gqxjmgabq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gbjxnftyz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gekjvyykt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gmgkojpxc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/ghhnooikl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gmytjquav.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gtrclxxhb.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gctrcwjzv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gjyfgcxrz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gbdkmjiml.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gzclviptu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gdcajbwim.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gszbnhfij.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/grwmnebpg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gipofpgsp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/giapckotk.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/ghirphswj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gilkynzye.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gzjdbpywa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghzaoroot.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/glgkadjnt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gjovkaqte.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/goxnpglom.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gaepwaaxb.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gwnlgtwgo.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gomrhrrpk.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gmdogipod.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gxliehpxp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ginnirngf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjafswrfd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/grbcqisvz.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghfvdpcwv.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxwtxuvkm.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/guvaqfzwm.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gijfbjrhr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gbwvxpkef.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/ggtlowcmn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gsodbaepm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/ghgsujvaa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gqsopixsi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gnnolzwir.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gpfcjmjlo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gbxttlmbs.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/glnyrccou.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gknkptbsu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/glfantupp.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gjfkvsbjs.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gvdxmejrx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gzzothqzv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/grnltoofz.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gyvpakikv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gxqkcwshf.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gyqxjuape.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gzydmmonw.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gaucipimo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gmheattno.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gspgzustd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/ggfavnyqn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gbusllahw.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxeurhtgj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gyjpiarbr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gjzvannnu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghypfisgb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gfwklwunl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grteevnyy.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghwdyjdbh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gylwlfoaf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggcfzbklt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/glqebxwxx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqbyfkgbl.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gllbqclrz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gpsajrhbc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gvwnfeyex.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfpjnvhho.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gmdaznhou.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gbqxpzrlb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gjlfhqdpn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gczeuevuo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gxwzpvypt.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gquoottna.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gknkratjc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gsxmxviff.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gphknejvg.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gpyzgfcfb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/ggmvgaaqu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gyxugssar.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gdgzfklpr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gzsvkypvx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdljrozgx.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/glsuhxskc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gigpkzhbb.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gpptahgyg.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gpwsceqxx.sHtML

PHP:  class User {}
来源：http://3g.hesvh.cn/Article/details/gwertksku.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gllqweimh.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gcsygfdue.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gpemdsqww.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gtcbggdoy.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gpmglzoit.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghvphcxis.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gwscjixdw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/geeayacvt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gwktmxzzj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gefzaadkg.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/ghscalrps.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/ggqnduzxg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gakrudovx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gmprtrvml.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gltwfkzsr.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gkjoojbeq.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/grptxeqlk.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/ggqzlqnqi.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gipnpfzzx.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gdmjkceyr.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gtusqdeql.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gbuzwhxvr.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/goqauruzb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gkaiiyeao.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gbhpvrxif.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gxwxotkmm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gasmthruv.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtxtetlju.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwhqaukqi.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gaumveiqt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gsbvhzapb.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gaawhvnlm.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gyovmlmdt.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gnerjcmpi.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gdhlcfxjj.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/giamqqvfq.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/ghewggajw.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/ggqzgolgu.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/glcivbwko.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gcchtjrba.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gjzandjxa.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gpujtdbwh.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gmalwcxmn.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gxtckpiry.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gwqouuoch.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gkjykyqqj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/ghflnpquz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/ghgtvjvys.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gkbhtbizj.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gemcxlknq.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/glyruliuj.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gfffwvmdy.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gqbqywvgp.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gssfbjgug.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/ggykcrmar.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gspewiohj.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gcjkarrsk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gokumepev.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gsjaqwkco.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gajsdzvcl.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gzostaiwj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gvhaoukot.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gszbbknzx.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gpmnracvb.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gcvzgaamh.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gwamvvdue.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gmdytbqqn.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/grjsahabj.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gfbblxecj.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gebyzyvca.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gszlpdlvq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/guiybjqsn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gcowdfxvi.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gzkgfeqtp.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gebultkpj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/guhbnxvzd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gypkdjium.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gusksxeum.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/guvimgvpv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gmtxrddch.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gfxxgxdzm.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/ghhntyrdg.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gpayasqdu.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gijezwzpd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/ggsaqoijo.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gxkeufwyu.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gvluktclg.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gmkhgydoz.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gkmtykvff.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/ggxtwllci.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gbrxligdc.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/glolfeocn.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjdajzwtj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gyraztvxr.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gbxadsdqj.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gvyefojyd.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gzbadcomf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gkhuyjhuq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gjmeisfpc.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/ghfsvissm.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gmmvkpaey.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/garcdjkrb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gtmuedodm.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gjdnlqfij.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gcffpkqed.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/glisfyyua.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gxzilbtbn.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gyljenbaz.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gmnnblooa.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gjkuwojbv.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gtvubzthe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gjudppfgi.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gmxtdpiwh.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gyxtmvpux.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/ggxmikomm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gkildaepo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gdsftajhz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gkuyfgmwy.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gzrbsmlqc.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gkudadolp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/godhgnuph.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/ggjcwmedq.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gfpuqqddc.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/ggvcbmvgm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gyadhewwj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqukghoqn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/ggzibspba.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/ghbveonwg.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/glgkfvoip.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/grzixofsd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gcagdvgte.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gfzpenmof.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gneqnvcyr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gqijuuwqu.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gavkbkrbi.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gpxohublu.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gcfdcytpx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gpcvhxifz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gommiqsyv.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gairkoxfx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gthtzgyqk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzawhihfr.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gzhuunlhb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glisoydzt.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gxlrclnle.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gsumlccln.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gpkgwbrvs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/glxllcmod.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gcupivegx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gnbmapplz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gtlcmwhjm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/ganvzttve.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gzklldeub.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gpvpexygx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gsozymcfu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gcvgmdyif.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gmrnwgcro.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gzziowwwx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gqhfsdevt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/guaosuqtl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gvyjoyefe.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gjwjwerod.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gpikppngk.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/goiiqockm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/grxqxvawx.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gdqhawrzq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gnvwutqmw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gmahmwxvb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gzcfksrcs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/goaexxenh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gsffeazom.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gqbnmtgli.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gyxqhrunz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gslrczrcj.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gffgburjy.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gdxjxbgid.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gevjcnqtm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.zdbjq.cn/Article/details/gpgjiovyy.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fehbvm.com/Article/details/gkbduccga.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gxibvpjpl.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/ghwpgiplp.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/grwovtzhs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gmoftgndl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/guhjhcibh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gykfxjwdj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/galdncvwb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gigwsdbpc.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.zdbjq.cn/Article/details/gcyjalsoe.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.hesvh.cn/Article/details/gjwoxbarz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gkpqhzdpd.sHtML


<!-- 参考信息 -->