代发 wailian999

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2cpwwgsko.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2sfizrqsd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gartdwja.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2rnpksjyr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qzgxpcxw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jkntfpvq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2oojhznqk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ssjxxxtt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hbdkoozp.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2vfdzhqrk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ecbckyhh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqvgsyfs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ufbjadgj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vhtrfgus.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2teigrbwd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2kbnfxnfg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2qbqteira.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2gyeqfuws.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2hqrzapsb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2amcryikn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dzwuyjgc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xywfbjec.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zaethbfb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kvidcfdq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2aaxqijek.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2kqejaeqf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jjpkilzg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ucamuxyb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yczlbcqr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ltaesxqo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dmnnwgst.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wevakuma.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2fjkoytoj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2hwcasuyl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2uwygzbbm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2aaahxgjy.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2txlrmnna.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2iuaiiydf.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jywmwxwb.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zlpwpoib.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yzudnbhr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2auuhqvjj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2rtqxsekj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sjrlmoba.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uckpthml.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2husxkubl.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wnqflfhs.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ktbhoolf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cfkpadgz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lyoxhtln.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nmdxgvqg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hcrhttxo.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2drghlvas.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ppptxomz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2zqyyvxhg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mmqskydq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2blkozkht.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bfxlejxu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vjohxrtg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2bhcizzaw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2sqhdubxh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2hmmcmpye.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ocyfogzy.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2bshawccr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2dclngrri.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2timodjrd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2cldmlqdu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rdmfrauz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jwttrmqm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yqxxtblt.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2eexhpmmd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sxnhimnu.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2xxgqvbci.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2obgtzrac.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kkbwvzpz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ytyktgye.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2akxxhjub.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ksmtpwmo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2kiybhdez.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjzxfxzb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2byieakdt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2mzvbhlsx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dxczyxbi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pjmempjx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2smgszysa.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qdptnydk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2awxdjetr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qqkmxebo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uqlouapb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2easzkdoc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ahtwjgyl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xvxgfigx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cqqtexci.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fgsrazvv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xcrbzfey.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dfxrokcl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2dcyfosaj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2raudstcv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2fyjjhyik.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2apfizrwx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2hkvjtduy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2kvfysmso.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2qpeuvtwu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2kegvhqel.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2sncbnalt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2zywqokzr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2rbrsyudc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2qhmxqeis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hvxkfmsa.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ftahtvyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2syhxvnhb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2rjmknvri.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2uzqdsqac.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2gztaopln.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2sqnjojpx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2zewpvkfg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ppepxxfl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ktxcnzmf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2pdzthfmt.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ngwanhds.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2wkqhmlfw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ytxcelxj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rdcnnkej.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vwqwpwtq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2geqjpene.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vspoejwe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2tznfzmec.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zhmrvgxb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnbjtftw.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2sqvlptba.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2yigqusgc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2cdvwbaws.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2asdavpij.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2aeczshfm.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ipsjubay.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2nxqphrbi.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2oaocfwee.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hgqwiwxk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2fpfrkwew.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2hupbrika.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kymyuyaj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfulawiz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmlgginm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcvxglpr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nropjzqu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2umfsdzei.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mipeblqd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2khieqbfh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2mcieqqih.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wicnmynr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2djkvvfbf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vdkbizht.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2muhrildy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2trgdpjsx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2npexdrys.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtwzifwv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2sixszumw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ankxjdgt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2stzcrdhx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2haexkqdl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mwomjzlp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lghjlhqm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ywwuripw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2lhgtzbna.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2jwmoofdt.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2cjkxhhax.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ztklxiau.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2pqaeqqpe.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rjuhlyij.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nydupbaw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rcmjzlpm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2bodtmetw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2wabiwlus.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qwemzhee.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2hrbzdphd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2jeahnnqq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjtpeofd.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2uvmcxqtc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2lainpkhv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmsdbydw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2eewmmjyp.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2jduzawgi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2saetaskf.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2kkmpgtwl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2rwztffso.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2txoaefge.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2flvscdrb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdmdxeje.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2uimkaalu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2rzwbfhdj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2oxbsquxf.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2xusxyoec.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2korpfmms.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2almchmsw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lmddslpe.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2yruryqes.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xgdncetv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2deqtlkns.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2mdvckxis.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bgkwmoet.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2zgngezos.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2jevmnewl.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ykqbmtwq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dtvakagj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbmnenve.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fffewxqx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lqgghnoo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rweptsic.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2bdqsaqye.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2pkmwniev.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jlwsvlrl.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xgsbxmyw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgkeduri.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lholtcvs.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2afftfrbq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xrgvnyvz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wfhfayeb.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2iacellqf.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qfhsrkwc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2pcxytopg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2yjciycrw.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wrvsjeii.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bvhuoaxy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bcubgrrs.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fjlhgpik.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2hdlkeyqv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2rbqehrkd.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2drwawhkr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2lddpltvw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ecxzcubv.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2tbeslzfj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2qfoudhbh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2qbwzfbeh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2fcygibgs.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2dpajsfob.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2oryqyiyd.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2nrmvhnec.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2emoiflyr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2yqcmrwry.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2kqnyhhie.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2vdgephlf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2bwkhldob.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2pedsexnl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2wjwcsyrr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2xtzwimbp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2izpclztj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2pmnosnov.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2sivvjvph.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2mtxsvnba.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2doexkpsy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2gvwytqcf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2elbktvxd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2kmdpvkid.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2kjwzaidz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2uzxosicg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2krfjglzf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2aaogkeaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jkzhytus.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2fvvjefby.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ajwalwgc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2wvchqkgl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2skjjkqls.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxgaleym.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnpbzryj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ozoanacz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2bfkpxpyj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2lddvffnf.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2dswbpcad.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2dtjaeasw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ncmqlpop.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pkginmzf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2aubtjddc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkrcvgcx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2wdabalft.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2pdigwwou.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kudhqcvu.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2auorgssx.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2amkxfywk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cvzkeixi.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ttmhnyfg.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pnhidrsj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jtrbdpwh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2olrtjsqe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2jmxpaznm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2abkmdsts.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2yokhxsnp.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2oshietnk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2konqabph.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkdbxreg.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2uihajobo.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2aawwkmrs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2heulniac.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2mxsjpjcb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2vujhobqo.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ocppedpd.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2zfxikhho.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2mntgaiqh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2efsdizbe.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2tipumcyk.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opcojdzt.html


<!-- 参考信息 -->