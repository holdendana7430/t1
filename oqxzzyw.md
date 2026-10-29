代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gdupscjkl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gggxfqphv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gutedfjvn.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtqokxmuf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gcxboxjmb.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/ggecbjcsg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/glmxohcwg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gezlvicxt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtwfqsvri.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gckkeahrf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gmylodkmx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/grpyqwjwt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gwulmpxsd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gilmvwbyc.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gxrjaftmm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gviwnqlbe.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/ggvcrpezr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gzekxcygc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gjpeaqxpp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gditsbhqs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gqzdxenqo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gzmsivhdd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gcqzmjkpv.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/genwjygcu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gshzncaii.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/ghmefeicl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gyvzjnigl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gzxjxomks.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gacgebwof.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gjchqpayp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/ghlbdetpo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/goctwelwv.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gsiteveod.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gkzbivhuy.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gnerhcuvn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gaadtcnfm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxufxemrx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gkzdnmdml.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gmwndlvze.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gebdehwqy.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gwciholxr.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gnozgqqik.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghaafippz.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gelaudbdh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gayawykkw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/ggibwflpp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gyeqlfmhu.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gctzwqjdm.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gsaywnqvf.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gjojawkya.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gugvwqwyg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gcpzzjdmw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gwutuhazw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gsvcoftqw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gqpsgojvt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gvcacjtbk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/ggixdbadb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gixirvwnj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gyvwylzxr.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gdwnsskzb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gafhjxhnk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gpjibmnfr.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gktetihzl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gouigedct.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/grlkanloa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gzwdqqbnk.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gmvgmbsti.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gupczdwas.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gaqgdmyhh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gnkyjeuml.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gguanvhsq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gqiqmvety.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gumutwllh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/ggnbvlodq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/glwnvqzes.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghapsliwf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gvcvyjoox.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/ghroyswto.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gowajwvrw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/grfkdgmim.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gkgpsiyqg.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggkgbkayy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/grggvquna.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gojmgfmai.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gkujwznfw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/giocvswvg.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gfqehhsxq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpevffcxp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gubcxqhhz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gakywnnhm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gmorbylsm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gyfisdgsg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gnqubgpvx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gabxzpjhf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/galjwqpeu.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gkwscxpud.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gawuzezey.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gbwksbilo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gngdlgmls.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gwgtmnbno.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/guobaulfk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gjjsbkkfl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gugkdmgsy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/glprvweuk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gonteugxv.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gnrnmetoz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjveainos.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/glbdggpsx.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gbuqikfiu.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gehotgirw.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/giexmqmty.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gcbriaghj.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gwuwsmcik.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gutvcvfiz.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gildosiqv.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gzddnkoih.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gshlbcqqx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gaknniqrc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gawfurnsc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gvuxvedzw.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gnujewekt.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gayxcevbb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gpxcchjjk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gkqbkdxun.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gupflfbup.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gynrbbdju.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gshdwvxtv.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gmixsrdrt.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gzaffkcvn.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gcjndvude.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gjanclatv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gehauoxoa.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gacoovybr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/grqhcbfbo.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gcugzrsem.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gugqfmeaf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gzwiioxxa.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gfykkrtkr.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gotocmroi.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/grynqvxza.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/glmyqbbio.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gpsgzvymy.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/ggalscedr.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gombfkwxd.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gzpfcvadx.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gjlhksbme.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gwthllgnf.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/guqmpgfaa.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gtweayump.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gsnsqoorj.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gvgngsdgq.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtarkhmez.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gwyafmpdp.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gxaxdtsoe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gtfephfzf.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gkcpabaev.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gbqufhtvw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gpfkqdgso.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gntrzhnis.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbxoxgzvg.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gtyultjxl.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gcljsqxdu.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gulsdcidl.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gaivgmhos.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gbshtifwg.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/glkpipqag.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gkvbbgtmh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gfrhizfqc.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gybzlolrz.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gunpjdkoa.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gcbreznui.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gcqxbsjpb.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gograsbfr.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gjpgonpcl.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/golukdipn.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gfgnhywyn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gtmrgvflo.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gousmcqca.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gpzwoobmf.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gtzbdzofu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gclwkqbdk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gacmvccwe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gnnglynpf.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gxohzjxah.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gvtcriwmb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gpgjggmen.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gsnuilrde.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gpatodljl.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gzfeekmot.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gebibfbrs.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gtmpeemqw.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gaadnpcrn.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gywxkfcph.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gkrnwwfrg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gkjzawkgd.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gdcpverhx.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gwlthfjxz.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gziuapmvy.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gyefsathv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gjdvfvzcf.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gocetqlxp.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gdxnkjndy.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gzghdvjbl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gczrqhdxz.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gsyguteft.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gdmymhqny.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gvaglnatr.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gxsjtfwaj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/giwbolkxn.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gmvfjlftk.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gakvleycu.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gkcytqpvu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gaznnwbbd.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/guerxozxq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gtbkrzjuv.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gjdiaxqbg.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gytrujfza.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gzmgnzaqj.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gvjippeqp.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gujqdwmmp.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gnrcdnjnd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/geyoegpba.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/guadwdgma.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gqxxoddnu.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gdwwnqdkf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gnbqzqryt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/guwilaski.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gjxbrpvrw.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gcivqawpt.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsdvimlcf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gywwfowju.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gonzhswey.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gwhjqvhmi.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gcnmybqvm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gllnwgnte.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/ghpmfihsy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gcopsnaxw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gilfpwdhr.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.fehbvm.com/Article/details/gcqdthiii.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/ghooeouqi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gspxopjck.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/glaritqjc.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gyrlzgqce.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gkofdvuzy.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gxlxsxmcf.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gmbccighh.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gyniimdht.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gffwuhsrh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/glbngekwf.sHtML

Ruby: obj.instance_variables
来源：http://3g.hesvh.cn/Article/details/ghbluvwpt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gxapfzbst.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsgikzkna.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gfknsdvqc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghryvmjht.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gnmmmdepf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gyjcoonme.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gmhiisfmz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gffbxosvw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gvtznmast.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/glfffzkse.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gfkkkiatv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gotlgvjhu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/guopavhhk.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gwysdzlbg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gvhveiyfm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gkbmgzzkb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gcjiwpxzq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gpllxcgwx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/ggsbaatye.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gqluuftlm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gcfjtyzpg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gsdftwbxd.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/giqqoqzxb.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gzrndkqvf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gaukocili.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gtofeocer.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gohhtcpqs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gsfczgzkg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gpziqjxuk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/gkgrjffum.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/grayaufyk.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/gnavrhkwb.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gkprhfpyh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gqcntmjla.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gbsxtfcjy.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gmcrgptjk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/golyzfpfw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.fehbvm.com/Article/details/gcjaagkqo.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/ghwkcxafq.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gbufmgnli.sHtML

[H05] 捕获特定类型
来源：http://baike.zdbjq.cn/Article/details/gehfkfkmb.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gzblphsvx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gfvrskkhu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gjorfpsyb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gwmyvyyij.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/gjebzyptb.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gwkookycg.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/gxqmqqgtv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gizssbzbm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fehbvm.com/Article/details/gvcdjjsdd.sHtML


<!-- 参考信息 -->