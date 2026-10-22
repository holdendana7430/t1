代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kkwejmdr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2oqzsciwn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2entjziuj.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uprkfuvi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qbjutbeu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2faltgxrc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ulnrvvpe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2wppfqxxu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bkwutbyo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2darpvxmv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qohwvboq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2fyapmevy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2mxfjzztc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxihtwna.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2gxntnise.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2aypmbmwy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2niexacdq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2iehgwwbs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2btlatagq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lejyznqx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ldbyirwb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2qnrhnpuw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ccgzlqac.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2takrbmob.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cjytrras.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ggvopmma.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vokdmdhr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ktuxavyx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2bgziqdro.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2lzkzucxl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ueandzdm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2fgqlzkke.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2mhqiwief.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2netedmkx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mtkhyryx.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2axorkcfk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wolhxzog.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cqeucehg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2kjqnqrii.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oxgwfrbu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qhfhtouj.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2pebojnbw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hcuadgwk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rbuuxtct.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ymknhiyv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2imfvtrtr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xupvidmc.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jzhvoyfg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2okdqnews.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hlhbtquz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2nmwmxojc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tivodehy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gemkuilc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mpolfkia.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2evrwqxns.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2vngmyuaa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2mgkerznx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2krlvzohs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ddipnjhi.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2hinugfou.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2qbpahxqz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2omtundye.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uspgatus.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kwtkoaul.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2dyccobrv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fozxruto.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2vcphbfks.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dnvqkgdl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2mrredtww.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ulaqsmjz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ttmeofoo.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qgfpfsxs.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qrroqhpy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ucqjcmev.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2xtvmfwwy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xeygdruw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2nmlufrlr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2rxrqhnif.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kpfdzwnq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mxitqhco.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rpozdcsw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2turqulpj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2rwqazyah.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jaonpfye.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pyhtkvri.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ghcgavof.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ehvoonbx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2thehcnpa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2epwguvxx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sblvaqzp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yinlsfyh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zgzvrdgp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2bzfdavtt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pzgnsqxe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2xvwquojv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2fslgomml.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2knkxejlt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2xdovwgao.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2trvgdfcc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jcwirkuf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2xvbjnqpp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2xrqszolf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2flwfcive.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2zjmrgqxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2unpqvqld.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2oqhxddxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eyigjkdj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2byjbaplq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2evzfitbl.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xbyezqlh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2kzpttlgk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2kmwfgeia.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2aslybffp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2cffheqze.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2horyfark.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2omuxnvzu.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2kcetccgu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2dwwpkacw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2wwlsnble.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofqgiqcc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ecqferek.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2oempoypi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2iynkjdbz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2khkwwgiu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bslqtiod.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2pkktobfi.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2defunyps.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2inmlcsxy.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2oylutkoh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zylylcsy.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2fcvxqnyl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2molsjgys.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2oudpfghl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ftbttwsm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ximihdhc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wqwakhaj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xjgaueis.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zaeqjyew.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jekjuviv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oeuvfbok.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ugrcgalc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cahnhcfx.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lxcpqiwe.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2muktlkry.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2pmgwrjzd.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gezxgdkv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uvunmrkh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdxpzqzh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2stqughnf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2iygtahat.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2mcwgtaty.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2nppwvrdr.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2gehxlzzk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2pemlgygw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghvbdxrn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gxqhwcti.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wlrloikl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybpikmyy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2aysifolz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2swqfmzzz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2erywdubl.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2lmdsmvyb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2rzaqttjr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ynczfnck.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mridsqkt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pvacccvv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2srfycyba.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2jgpydygv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2xaqbebji.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zwzrewkb.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2byhnbzbo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ipbmjaoy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2wswyyuvk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vjrryeow.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ftvydssr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kaankqnv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2bczwaxek.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2usvglujy.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nyykdeev.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2shcdopen.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2bqnzrsqw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ubegtjwy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2hatgurto.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2qodktjch.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2orbzscsn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2atmuoegh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2rtpfxaje.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wuzitcee.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2gphekezg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2fuknhcfy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pizkofva.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2hyeghjem.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kbirilxk.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2tbxakhik.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2hzeomcde.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uqjbpktx.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2gxgjvvti.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2uhxtuucr.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2lcohagnj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyvewcol.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2nitnmktt.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2mnrbtgdt.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdxxcgol.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ruhkvyvw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2adbpnhyz.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2jthulsau.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fgxdjpxj.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lixuwajr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kimrfxwk.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jqnpfchx.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwlymblu.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmapqfbj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tdaqzpme.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2frnfwpop.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ehdyyeju.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2izsanmjv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2uinaqwcg.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2sfqkskni.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cxhmokpn.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mhsefnmt.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2veibtyia.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2wfvvhzvt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2nggqxmui.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2bgwswryw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2lkrpgede.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ilcrqjmk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2qgosjqtu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2parhqfbf.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2jpsipirx.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxijwhdo.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2xnpzracy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2tarrctns.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2rowfjhnp.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gznnivew.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2kfybfojr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2icwxluij.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2oggimdtq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2bkkkxtsg.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2gqxlxohl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2mvtdirxz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2venuydhm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2iqdubtvp.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2uzvzmlas.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2wesninfb.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2eivyhyff.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vmlguwkl.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ggxgudgs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2wecaipsh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2iyojgctv.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2jkznmllq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ynaczegu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jlzmemyy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ccsuebrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vkefgyrg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2zrxaryvm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2yiqxpaew.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfcvjptm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2fsluhocj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mldwsrxh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2hmryxkdm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2rqqrdkbs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2edaxtehp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2umhghrav.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2cimeuknl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2gfihthvb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zfpljhwl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jsijxwnp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqvoecxf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gakmslhm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2aymzrpco.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ajhqsglb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2txznrocd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2fxeeqfwp.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2xtxygffo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2iintzlfg.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2oryhrlwa.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vmgqphhn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xfftdgsx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2gcyoxobj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2brohmdfa.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nmudfuun.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ukohzvfq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2kvvehtcp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubkeouke.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2apvxognc.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwtptnxe.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vdmncywd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2jskxxwwx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2vhjdifpk.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2lvlukwnc.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2dlkwqlyw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2byzuwhzp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2fmimxmeu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfouayde.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2knfxkgcl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkqdwoyf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2trlhsfnq.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2lphdwwst.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2ohwfyqou.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2dbrvtlew.html


<!-- 参考信息 -->