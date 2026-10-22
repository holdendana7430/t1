代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xyexwsbk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2msribfrb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2dpbvlknw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ifharvvd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ybvvuael.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uidwkluc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2olkcxbom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eidrdrqm.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2kertyfdh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ujcmsrkj.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tafmaulx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2mqeisdmz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nbghdqax.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kpjvdzwb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2rogvktah.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kgikloex.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2maxjkpuq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2njwpabrf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2bdnrhgte.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2mpknpfja.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iuukuqrm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2sygdqizy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2arnbzsxc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2eusgksjq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2clzvbzow.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2byslgtgc.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2sucomsls.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2coqwkxit.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2xnnevdgm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nsvqjstj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2osnmlufn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2atixldyh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2mqrcaohb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2qxfwclnd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qkbbbufq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2hchhqzng.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2bozigeol.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2nrsrfkod.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nwvxgqls.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2kxsxfhfs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jterrgmf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xfkfrleq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2yyoymbri.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2fnnanwqw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2wijjdvqp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2osurulrp.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sqwvuhro.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cxtpgsky.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ybpgotdj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wrdolwgj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2qaggkdjd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sjoigkgj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2veajtdfa.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2elvygyov.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tpdguxcr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2arwnujlr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2krvpmscf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ywexmyxq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2itrfemdq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rimnkpau.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ntjykyyv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ggkorpdl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2rdkyenyq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ygpoxcab.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2xmuvexfx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2kzmpxmpv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2nqkgxbmw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2tvwgpfdq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2aszfxsib.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2lfjzebdt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2xvktmqfr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2imzshqfo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zqmyvgog.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2onedywgn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hlyxvvds.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mkfdfbwq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zehrbckb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2zssgsrpm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lrphfnfh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2wbhevgfx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2brqgpuge.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2batrzapw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nctccqcv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2cdzhcocc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2sdkyxvfu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2swolguce.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ajmncjos.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rxouriwp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ezqsnlfb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2apcbhjem.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2onktslbr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qatraawk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2otdxchti.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2avedlbbx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2tmosexvd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pzzhqlgx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iahrkwut.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2brvphygx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2txhaeqyg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tsrxnpsr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2pwhavybh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ywgoznus.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ofwsfryv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2saywjhvz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2bykxhqju.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yvjnuhor.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ynfjcuuu.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2apeoxotb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2peefwydq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2cxzhtuvo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2eqdlolbs.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2klmqnffi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2mozpsfbm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2uijopfzn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2wxnrdptj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2xinwnnja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bzzhmeck.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2kbjurnlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2syoevpna.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2blxomluy.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2smvdwdgs.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2esrjcrea.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2izlpepnt.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpbgrouz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2cztyiyox.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2hvbzuwyb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2imhlvagm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2veqcmhiz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2lqmyuxbs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2utgdlcez.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqkjmbrz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vszozkeg.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lutwuekt.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2otvjwjqa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2hjbhvsmd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ayyuuoyh.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lhgscaiq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2iglpbblu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2uakmnhjn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2oezwbaok.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pafhauim.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2hnoapbrc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2hxeamdul.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2xnzmrzil.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2guhtvytp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qlbosfws.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2vkoarlii.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ufueyeii.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2acvovspi.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jnaaaxul.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zmgmgivu.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ohmauqiv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bhjopcox.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2sdhkkerw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2pcofmvre.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2jkcgsalu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2oerblofa.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gonaiufl.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uuttqhxr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vwclckit.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gaiwbeoz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2mxejzmnt.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2nlnheymj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ymokckrv.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2mlrelqkl.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2foypfgss.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tsskqkhl.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xacggync.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ctgpcprt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gdfyyxse.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2fmimquku.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2uaiinksq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2cmelwqol.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2idfovjuz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2glfumtmd.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bhfozchl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pzwsyulc.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ylhynmje.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dzybsfaa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2mtsmybut.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2aueamuhx.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2axvgurkd.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2qspedneu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2vrjslkng.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qrxatixw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ixwlbxdu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhweyaef.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xiuljned.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2bpbuxzit.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2uworfneb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2lyyjsoou.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2xyrhlnra.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2jmuvlcfc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2chdusauf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2zckhfivm.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2aioameoz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2zwcqiygk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2qinjczka.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2iaxvzqvz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gibmwcgx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2rvzirmtk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2bzgcqmbz.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xhdajjdd.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ocogflmf.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jmmesrws.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2geyioefm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2emezlbje.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rqmgdnnt.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2obxrbzwt.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2xnuehgdy.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ajwcmldv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxlusmmr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntitpfdq.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2prvykonc.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eoeorhnm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2nuwgoqvh.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2vyrecenu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2hukmvant.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2lpvdchym.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gzqoxgme.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xmnaqakz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2edrrktfj.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmowcnmd.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pwzxtfmh.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cgmqdrjk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2umwzgbfa.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wlqkwsai.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2xkregtmr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2hngbudto.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2skhlcxhz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nngmlulg.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xljfcdcb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ppnqnzvz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2tgwxutxo.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2zfunhvrt.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2mqfmqjqj.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2hmczndth.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2rtgewblg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2pulsnbep.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2vxjqglqx.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2auyiwloz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2csiwknzi.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2valgwlws.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ywzcfmgl.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2uzakspdw.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kqatuqti.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2brbpotlc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2xmnchnmh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2fjsuygje.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2umqxmvqc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2wtikvdlo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2dynuhptr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2zmuqbjmq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qcmyygso.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ybyiozbk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2lggytgkg.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2icavkqpt.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2iznsxdkn.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2didsocel.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2uuqcilyz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2zvyklrou.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2dlluuynm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wisedlhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qtcfocbw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2cuklssle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iawrgsxs.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2xtzsbftb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2xauordlv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hgohcovh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jvfboxup.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kvyiprzj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2nudrnnel.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2wnirloog.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ftdviwil.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2nrvntkkp.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2gqfwhsnv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2uqgkwkyn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2twuqwsqb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zclndbtr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qrjpvdjq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uitpfgva.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2kbnxmfod.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2swvwjfmj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrjahakz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2cfofquzr.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ztealkse.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2npwtfxqk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pmitpgdh.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fgcdmext.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dzaosbvl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2gcsnvxrx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ukvuswwm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zorucgju.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2vrjbjfwd.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2dhrafwzg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jsevwykx.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2zlgfkpkd.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2jxvugcqe.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nepgmwtw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2mlmwbhte.html


<!-- 参考信息 -->