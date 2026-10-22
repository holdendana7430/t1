代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2rbvtjxdl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2uvtxcajb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2iuesexqt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2liwjzurg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vlflskwy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2qdypbbjd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ylbkezqa.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2otjygxff.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2nhbyqwvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gcsfbolr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2qxceiiou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fduymtjz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ccindqab.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2aaoewagp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fwfpxyyu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2fpjczaxp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fbffrdsm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2idiptczi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ufgsricl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jqpqzvzj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wtdmtnwz.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2lwiydzfc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2cveebyic.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvwsfilg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdiivdew.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mfaanrsj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jaukiofb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2cyuxosxb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2yhxekohk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2vesreclc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ichpamgj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2qsayupgi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2aafxkshg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rphymyxf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hvfwbuie.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ytifdizi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2qwozqyhy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2hwzrzkoz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2imtlfoba.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2vkpelinx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xyrmcnjk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ydwtnpge.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gcksbhoi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zprwfrfy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2brnotpfm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2flwppaqq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2rrfmcrdw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ddcnxzsp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jwoodktd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2dhgrdexj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pbzufzge.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fpytjuhj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zezjmrvu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nwvxxsrs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2iuzjuozr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2omfsdsje.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eofjzfbr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2xijsxvas.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nsphhxwb.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yxqfbbjq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2drkcarly.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gvodnxry.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gwtoqqou.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vskgwaye.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ytbblmhc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sqizitik.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2sbvdisgx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2axdrfrdr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2wosnjuoj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xeyqcyox.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jnwacckb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2vfolqfan.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ecjsnqsa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2pdarjkse.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2mbubllsk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2kvogvqwc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2fhxmuden.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2bvlpagvg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nylifbgz.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2qashsblo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2mjeahbyp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2clqjldud.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2iylobnyq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2oamjxryw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2bknvegij.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vtljlhxq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rhznjpkf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2izstrpax.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2miboqink.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wljlrqgh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2hikbghfw.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hvemgkfo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ucsrscjs.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2kulxwkdg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eeldgved.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ozgfeucs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2riunrmfg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ksfrmvfj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2qkostggx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2javstqrf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2liozwysz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cmqrttts.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2gswzzaur.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qojkqxcw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jgkekmzz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2imyqqsrj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zofayzru.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ipzuyvdi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2wmkhmqrn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jlrickir.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2lbhjwmut.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2afuudlkm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2btgvlyhc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2cngyebae.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2cnsgrdwg.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ffdrfgtk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ytnjrfve.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ubjrvfsx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2oeyxuuvu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2qspwojfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yonmqtxr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2mcxjvhyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmrosxjf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2mmyhctwo.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2tzsecqka.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhcqetqi.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqikuswt.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2jxiloyvw.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jereipjy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2dekccbap.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2dojzcngg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hkxwlvow.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gpklmobt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2iqwyqjhl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bejbhqyv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2digsokit.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2orsgnsue.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwarafng.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2cxiqphsh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2knyvaufx.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2oazyzppw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2hcujsjle.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2idvihknv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kawcgkvv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xnxscytc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2krajfsri.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2uyzlydfi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2jnpxdqhs.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fhpmtmgi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tuyodbaw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2fumquknx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vpomtelr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fscerdlc.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2henmbhpz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtcvcduy.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwlqfhus.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xmvenjxk.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2hdavucxd.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ybvgqqwi.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2yaykbtkd.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2tmonwnnm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2meooezdt.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2elksjxdk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fhtbvrsi.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbscmnlf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2fsanqyor.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2hsowurtq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhmadtjc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2tqgupjfy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2uosckrkr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qohvduux.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2aqoiltif.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xydgufuj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rgoqetid.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2hwvjegxw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2rdnmapap.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2tswdcfky.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2akomqtrp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2epbqfxoh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jhgaqfpg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bvyajzxs.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xolmljji.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bzycfakf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2dpamfsnp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2odczoioj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ngutiphq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2arqpawsh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2pkabwrol.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfhlbelh.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ejhsidqj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2bsxsznrq.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rbqqlvqe.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2fphkdheh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ixdltwsi.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2bbwzkzep.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2wecpmoav.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2sjakskyq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2etoyxpor.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2lastimaa.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmsumsxd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bypxcchj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2fquppfsr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2gazcduky.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2mztpyuqk.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2wtufkekn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2mlxwmfzl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pflfjsrt.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2eyljxxrd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tkkazovo.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2tbgseqsa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2brqktugb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kvkalaza.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2oxcwzcej.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2epuvgxja.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2rvhhmmel.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzzcynws.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2syviqxjy.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksqybozx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2twtqzeds.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kixkwtpg.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2mmjlvobl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2yyxlbkzm.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2czrckuhw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ztkfnxgv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xmsgvzoe.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovkurohf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lixezrhu.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hptfidcv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rajfmefq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2agksyacd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jitnfxcx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2yvgisoug.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ggvpqchd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uahkliny.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ibvpdtfv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2slkietsh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hueuockv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2soszodhb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2xnvfxham.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2nlaxavqh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2maghkgpm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2dwixdfif.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2slqxnycs.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ptaifdxk.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2msmdihwh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2mzwhewvf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2xqnemylm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2conxmiml.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2lvimnkyz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2blxzwchi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2mbrgfprc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2pewgprer.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2pqugyfth.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ggvvdkxa.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2fgfubhhl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2mmiynyni.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2sqmtrwbt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lzgwqrnv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2xncrnisr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2lfzkuazl.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2zmkdfivy.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fljhvijb.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wnznirfc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2mswlnnoc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2vyzougdb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2bvvqfwph.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2bimomelx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lhjqhvql.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2hsslcnor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qshxiwsg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2nljqwhgj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2hzaiqeww.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2aaujgivk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bmpkgcor.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2odwwjmcg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2yqwzsswx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2aljkehye.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2qmregxrw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2xgzdkuas.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2dofcsqvd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2pobjlzmw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qubmyjyl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndeuenmn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lrtuogkn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jrttyfib.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2atszlbjm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ystfdtwt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dagqxqpc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2dhjoutwy.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2dxwheshe.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2dzhxcyfv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qkhnsidf.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2arztntea.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2loxspyec.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ahusiwiz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2imbqsqmg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2eochgdhj.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2fvkdwunt.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2uuniocbc.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vdyychgo.html


<!-- 参考信息 -->