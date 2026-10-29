代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ghqkpbrwy.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gfmxlbvkz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gcjeeztaa.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gxdxrzncj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gwrrcbcdg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gokxtzvif.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/guaytnwqh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/ggrfmsvvw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/grtgqyqus.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gdgcpcggp.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gipuccwcz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gtbrcqttw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gdekhvaux.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gaxhdxgdu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gtpkxpvcz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gibrvimow.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gilepwxnr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/ggbgtjqlf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/glnsrciuq.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gajqrknqi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/ginfevpbe.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gaufkyoyv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gouciadhq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/guxtjnktb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/ggiwoosyl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gpngdelhq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/glmbvowww.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gijbphlgr.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gzexsuoyl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/ggetsvmlg.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gvyldvagc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/giswasihl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gflbkeskn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gibyzbqze.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gfefrblvh.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmdixikhd.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gadmjoirx.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/grsfnkavh.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gvuclipga.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gbnfzgssr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcpyltoql.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvkgtbpnl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gbbhkjqcm.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvcyhghyx.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxgamnrio.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ggtqtfmqo.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gvpvtjixj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/ggplbchys.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gmqqoumiu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/ggpcmjipi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gefnkhfjr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gpqsdkikb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gvfinisct.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gzlazsnag.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gcxblbiwi.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gwjrfexek.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgjibmpz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gtnlvafgt.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/guumqrnoo.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gaaxxzbgt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gukeraacv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/giialirif.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gmdbypewr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/ghmsmogdq.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gyrnrznnm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvghqeruf.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gzctmrzdo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gsyubvymq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gwnkvjgtg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/giyebiprl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gsbzfquxl.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gakmtqlvt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gplamralg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/ghsogleqt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggizzbqos.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gveqeedrs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gedtjtsyg.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfkyggkfg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gqszdtqch.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjxsdtmow.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gopzcpmtx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/grnxazdjr.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gcieyjzsz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwoyfsmxr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/ggsvuovhq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbmgtsvbl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gufjwvcwd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gwiyfbovo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gaslvamhr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gyaxlxyfo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gpdcfedqk.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gyyuwvxnb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gcuryvflu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/grlnxjgvm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/grmqjpkxq.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gswkaeaez.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gbcvbydnc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gmhjzrcju.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gggkjbquj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gatfbjqhn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcyctubco.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gsuuralmo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsqbwkafd.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/goraunuin.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gqimssfiu.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gxsngtrio.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gizifvufj.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gpgoivocy.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gfrqrchhm.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gjklhkalt.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gqiqgoagk.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gmyiqldma.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gfcbccimk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gxzkdvnzc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gmfkelsgg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gxkhxumqe.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmqakghgb.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gsnwnvdtl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gcozcbsui.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gzavytnip.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gztwkkvrd.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/glvwttbxy.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gvbxrwbng.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gziaikxeg.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gnugrgxnm.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gnacsqocl.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gphyzvgho.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gmyajnlkt.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/ghsfmczjc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gqvmxuabj.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gpyyftscg.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/geruwgxsb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzkxoevff.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gsjdqeyld.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gcydjyjlg.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gtueqetqn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gwgvzhonr.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gioqvtccv.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gckrgzcfm.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gssfplbca.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gpfvthnuy.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gyabsfgsw.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/grubvcqls.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gxuqnaqkg.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gtrfjnjru.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/ggufjlosd.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gitkjnzya.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gbehlihtl.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gmryipxwn.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gnrudapxx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gqzpozvke.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gvbsquqwc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbkwxiqdg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gdocqigxv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gjdxoxziz.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gjgbwzfuo.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gikemboxj.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gdyoixopk.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gxjklkqgp.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gxumegzdd.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gxxtaydbz.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/ghwgotinn.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gwtojtcrs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gninkkokx.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gkyoyawvj.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gpzewdhpp.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gwtievwdi.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gzwssbejl.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/guaapkpth.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/guvlfglxc.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gjoqfpvcb.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gzlekfmet.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gqxmynnuz.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gopbfadbj.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/giyepfios.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gqlbiqnjz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gnjrvfkkf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gbiseqilt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gdmhfjdgs.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gxjorztpc.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gwtgojeoa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.hesvh.cn/Article/details/gvjbeegbs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/goxgvcdtb.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gmiyahrbz.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/grsoeujks.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gbvwaoych.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gbcnhrzly.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/goalqqklz.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gsfeejpvq.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gvcpwqrhe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gwxtshjdy.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/geugkzixm.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gppshpmzp.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gyqeszeju.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gomqzxzqf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gblfrxnhb.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gbfstbhau.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfmjplmao.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/grgnvdzhy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gvkndnjjm.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gvtlekwip.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/ggycavrul.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gsbdafccw.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gqwligtxf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzgqgahny.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gtxjptvvp.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gjsxsuvjf.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggsegztdr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gcjrsdwzq.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gqhszibsv.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gmqvfxizv.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gixnzablb.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gcvwgbuab.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gcfdlhgjh.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gugujfitj.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gkvcjflec.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gifyappvq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gumxivcse.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gsgrvkltr.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gtkqhuphh.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gjpeybgxj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gbxlxbbzq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gcovoqgrj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gdljktnar.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gigtvsjde.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gvstgufwl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gtxxyrtxo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gklgckwec.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gipxzufcp.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gocytlvhu.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gjtyvkhgw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gumnxaanr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gnqxqrtcq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gpvuvrgrn.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gltmgsxpy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gqrkaiuxb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gowhssijo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/guhxkbotm.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/geqxygeet.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gmmzpdnjs.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/grurynxsg.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gyvcqxexq.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gngftwrvs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gfjirhree.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gdthhxgsm.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/geyetnngu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gnbxsgsdn.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmrkkzbes.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gpkgqbdww.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpqgennfv.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gqzawavry.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gfiiqpxgi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/giehvfxht.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gyfcjpabg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gtxovmaxn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/govwodwsz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gswkpkyui.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gujqkpbdx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gasdxcqak.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.fehbvm.com/Article/details/gynxfdaei.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gtbesquij.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gapyrlhbw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gkgzryebc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gkyztlchl.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gqvstnvjf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gwimpgaeu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gogwuqigf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gwzooploj.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gsrhmqihe.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gogemukgr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gzvzwmuur.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gpcqpjkxu.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gseyvyfhy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gqpjelfrr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/givicbqln.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gczmeunkh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/ggtrqtdpa.sHtML

[H04] 自定义异常类型
来源：http://www.blog.hesvh.cn/Article/details/ggzjahtmy.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/golvxcoxj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gmflbdozy.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gxokklsmr.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gjhhhrkjd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gzfgejknz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gvhwbxecl.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gpmrszgzy.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gufdgmrbt.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gkmobakuj.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gckpjegvc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fehbvm.com/Article/details/gucpdxwgk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/glxqlpnfn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghfxuzsan.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gqgffvcrg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.fehbvm.com/Article/details/gqfnakdwk.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gossnjxpa.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkrdcpeqt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gibysddes.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/glodoqnrd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/ginwwsbwo.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gwkbnwrac.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gkzuutrth.sHtML


<!-- 参考信息 -->