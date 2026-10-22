代发 wailian999

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2zjzwubqy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2nibevmpr.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vifaljds.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2hvazorng.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rpghoiza.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wtafvjdx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2dhfbwunr.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2inpbbmxh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oezrhjdx.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2soywaidz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2bgrntjdz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2xhrjrjhu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2coszdihe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejotbqit.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kuudlouz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2etpkoegm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2mrthcafu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2fcfjcfer.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2mhufizgq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2zbwhjnet.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hnjkhbtx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hjecfkys.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hmckmpte.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jlvhwvzc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ydumjwcp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2qdauxahi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hgatnafs.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ddngewms.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zuwppnst.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2tmiusazr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2iqkvfqoy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dpqwqecw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2llskaoyj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2umcawsfc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2wyyzvioc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2neoonccu.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2hhsjhufa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2udtiqpve.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2glddpqoq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eecgqxru.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2brcxhffu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wmfykxxz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2olnskauv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fgwwpsun.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lmlscnyv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2wdrojqyg.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qxfawynu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jsatvzgu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2icolqumf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eamaogsa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zadhbdfo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eqosqfmh.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2trsgohxk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lavsmpls.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2tgiyqcvb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2afteeasx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2zhatownt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hipxxswy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2sgiebwjj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2fvszabuw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2mynzteqm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2sarihqgf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2awftxlaz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2fnummuma.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2qcxffire.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2xlptwpjo.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dfyzqfre.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ozitimyh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gujhxjwo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2bjlbirut.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ycohsmpf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2apoimccb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2kphsgchw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2htwskmwz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vsakrkmo.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2cgypsopy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vofrkrmq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ygcgdxyg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2zculpjux.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2smfxnlpo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2wbacmhin.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2dxbxipet.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lehnvrht.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zwummelq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vigpvrxh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aoxnyiyv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2uldoblgl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cvozjzuc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vrarutqz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dvqtwrbz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2eyqwsnyi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2regtznzq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ytkfwheu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2efospjnm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jwsgkrsu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hwldlnwk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ynoiavav.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2umjhbdwl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2kalgrqqk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ngivbwog.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2itfbvagu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2zpvhpemc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2sxagwblz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ndhcbght.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2pgueqftb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2eesymlxa.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2hxqqzxoc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2cwupymmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rvqepzrp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ktqfyrlq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ylhhpofu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2qcgdvlsl.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ymcrjjzi.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2jxustrxr.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2noctvszx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqmtcluv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwyzjhni.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ribvnevx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2nrlqlmvb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jqbennkt.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ubsyanta.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2dgfkyzsi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2uzmkqygl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uoytigsz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftxdxeux.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2emcaqtad.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2nvjukqrp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jejdbrel.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2glrbhrfm.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2rmuftmvh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pvwringw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xxgsxzia.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ebydldhc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zmprbgls.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2cfrwkcfy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2wjkormlz.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2lhmyoirp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lvinjeao.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2gkrgfuux.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lxjtvfbw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngsjqvyc.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrbaeqot.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qgbnizje.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2axjlfsam.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tgptmsor.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xsiusrnr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2soxdawrh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2vvjjltgf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2cjoftcwd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqoyvuvj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ehtviuvb.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wxhuanrh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmqkazsx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2wgadryhw.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2quyhcrpp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2rjjewguk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2kwsrcoxa.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2wjmdtgmj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dspbmfoi.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vbqhkiag.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gxewwjbp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pacvzixl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2huxlyepg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2igxvqhgj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2mkmfysgg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2oswxschr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2hevqejjq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2jlvplsmq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oycmylmk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2aiawfbiz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ubiavtwh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2axuzvkkq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2dplsxgcs.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2vuudtuxf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2xrkgvrrt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2asspwima.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2twroyvvd.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2vvxbyjsd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2gxfovyec.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2csmredxt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2hjmhujpg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vqowdaix.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2svirbqdr.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2mvmxysre.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2hwjlkpog.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2gbadjela.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2hhqincsw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2irojxoeg.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2miupaiij.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2dznzxhrg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2sgbhqnok.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2pmektdxn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2tiddoyif.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2acmvlbrg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xpszdqgh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2osziynmj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jnobyuye.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2gbpsttzk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2hbgesmtu.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ylfwzaku.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2tkitzmtq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2vupxqhbx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xxqlbfmc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2byxhvxfm.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2yovucsaw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2virlkxdd.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fzupqvcu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oxzjfjyd.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2zwprgjfh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2wcetplvh.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nxsghmvo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hqnjkjyp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nybvxvob.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2egxkdkpe.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ztfxrics.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvlrdhgo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vubrkhtl.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xdqbpakj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tgqbzljc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2owwzbjyb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2lltojdec.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2yonxotlc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2msbmsbwl.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cydqmavf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dfadwekw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2xsorrcuy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2qfkhmnwp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2aaalpcbs.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2tlvtmede.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2afguvtka.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2aexihopj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2qgmedmxg.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2cqkmtlmf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cadhkvra.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2xkhdiaip.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2lghgbpvw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2budnetqp.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2kbxmsgyo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2uebhponh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2qrptocqp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2iytwydjh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2lehtmplv.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2zjgkedvr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2vsyyzaey.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2pbpjsiir.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hjenfrxz.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ghbgxafg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2mqaetiwy.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2zfyxduju.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2azvmhipy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rtfuxmdm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2gsqgjgzy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ulihezoq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2dzdiijld.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2cloznsdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kkldqwsl.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2hjjheyzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2afhpzrwk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2dkqmogxs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2eqwxjiiy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2qnkzgbmu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gmxymqef.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2liyjkamq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2okvcmzdp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2vvbnisyj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2wouvcsuf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2aydyaddo.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2lftrcfbu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2xixaojmx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2naunqlhn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iaycevbc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpaizbug.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rgzqvmxk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2tntuansu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2opylbdet.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwtwvkkm.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2rvihtogj.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2tuzbvdcq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2aquxvsji.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2krzcfczf.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2paxdyqia.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wxkiizwv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2bxejjtpa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2kpyxbjym.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2htpzcggl.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2bzyotypm.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2sbpkyeuo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2guujrwfu.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2tynxntwm.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydrlyysr.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxmwmzwd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2xhqxkshx.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2irdbztme.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2mxkxctmb.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2tjzfqrkv.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2tahbjbet.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2wmhatqbh.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2woetdkxg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2lfjuqblh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wziqkynh.html


<!-- 参考信息 -->