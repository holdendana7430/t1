代发 wailian999

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2rfjxekwi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2fuvhodqt.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2boxaeidj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ecdopgha.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2seizkevf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pwualypr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2jvgpjhnm.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sdnqyfvb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2noibuucs.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2geonfbft.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2gzouyybt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdbnfzeh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fbwgcqzo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wrejwjop.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2lipibibv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2vhbeznrh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2wgfsewlp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2pnwgvmde.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2jdqhukky.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xdhbyppr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ofwvzmjy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tpiflbpj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2pvgwhrxx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uhmocmpq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2eknwzurq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2atcefqfv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nauofarl.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2xlqkjdkr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2oqdwpwrw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2dpueccpn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2agjcerkv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xwvuyopt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2qlmmvwdx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rwqfwvuv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ovuyrfyt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fmtxwnir.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2fmqplrxz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2pioyjluy.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mihalpyl.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xdxxycvr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2agqmtnun.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cbgkllmq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2tgunucba.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yuczjjkr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gaipcaxb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2syadlhfg.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gukwyuqr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zjyldhes.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kcrhafwe.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2euqzmmoi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mimtgids.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uuyrhgvp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gbbuwsjh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hzvehlqt.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2bsymhbxv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tdiuzsya.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2gzkbfuwu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2omitafod.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bdnnwawv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ptpsmpgk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2sfnohhny.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2xisaqmxy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2jpurisho.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2lnkzplay.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xqtdbhdv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2kkepyzmi.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2qxzzfrau.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2cwsevcbo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nycqtmdk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2egyqufsz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qtfojldr.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2axhjfuva.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2rgzgnvfi.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ugnxielg.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sjgfeesd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2kdpnghej.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pzlhdqth.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gahuhmzc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2zhayfgof.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uiqcqjdn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2vqempdlp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2gswlbcvl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xozwgdpj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aihijcta.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ehrbppjp.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gbauvjtz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2dsqueyod.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xkgyuohi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ffmfpnfb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iriicfir.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2sedsdiqb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ongvmmfo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dtlmtreg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2snheywyf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dougsudg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mwhrzcbq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2yylhixsl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eazbuozo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2bcnptphf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2edmxgljs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2todoetwq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2rgoepfss.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2unoayfiz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2umlwfqlv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ftfblwev.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2dxdivzng.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2xyblrnup.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2iwflvvrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2knkrbenj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2qleuuylk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqjjfcsk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2dnzrkpqz.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2sckourfi.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2htjxnxnc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wpdxlsun.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2bsdtscdo.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2zowmkrak.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2nelukegg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2wiwaklmm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucemugix.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2jbhtjqpq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2hmtexybs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2psiuahwv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yylttdeb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xisflddi.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2afmumuog.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2wjuhqyhg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2yhfdsdya.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2durfbiwc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ljikuybk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2aqvoxtwi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ioqovbdi.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dinhjgdu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xjavgxuy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2vkltbcml.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2bvszrrxq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cwqhhazj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2hhrifczy.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2xhwtsfpo.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2iplerszc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ouzzogqv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ypztkizb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dgiggwnh.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kfqxwajm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ikpkgrsu.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2belvouyf.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ctjvanyk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2pndaqdmj.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2klyboont.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vnjkjkdw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxvcksvf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dbsyuxxl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lzvjroml.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2wnknifdf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2bikjyccq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iksjsota.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ousjphwg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2owhyfmkl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iahtasic.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2beulactc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jeusfuhs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2swnyxqhg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2xgasedpc.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2zbnvyovo.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ghjzurrw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2olvowcfl.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2sxvljnmj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ncuvbnoh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2epfyhwbo.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2umapjjxu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qqaomhxi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2svdbtgdy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2krieasyp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2mwuwrowf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2czniobra.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2piybufin.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2myydysnk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xukuseyk.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2wyqknqhe.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ovddngeb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2xifikuqv.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2hqakginq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihbdgwss.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2udtwlrnr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2skeenugh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2abrzqmzl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2copeukvn.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2yxbnteiy.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2dkortvux.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2qkfdqdxw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2jybeamlv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fvrhscbk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2tgpvtwzv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2aivaqpgu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fmtrljdt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2aoprkmuq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uqpdtbwd.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2wdbjynhv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2nxviejnc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2okkwytlq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2mlwxqqoz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2nvkmoses.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2azoocmvs.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qbezjoym.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytzusfyp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kssohuof.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uqhjklwo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2asjhvnmc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2rvzpsgyy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2tsiwsclr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xxjqhova.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lhdedtro.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2yvzkkazy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2szmhkrnb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmnjaqrw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjelrkuc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lepgdqrd.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2hngbsirf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2darmpdfk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2iafrqoki.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2hvxdkhnq.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dzfyehzz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2trmqoktg.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ftsohgyc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tsqeywsz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2esanlqad.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2spgvrvkj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2vtpzrqbt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2sixkhlxm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2yphndims.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2noyhjeax.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2imblwfez.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2kjvrxmlw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dyjovtjc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2tfqykfae.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2sofczlkf.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2gpmglfqc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2jmhkqjwk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2gjvrmdfm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpdawfxu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2zbhmdkqm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vpkjdncp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2tpukibzj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2rmupqayr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2wdpfksnt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cxyxdiyb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2mqlyxuau.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ffomfixd.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2xriqpahp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lkixfzky.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dpwfbivx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2jmtmkdbw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2yzqehghr.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2npuaczyx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2cmaiyfpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kmvxfyqh.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2algzoxne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2suczxtey.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2yljlocli.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2worxrawp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2omadxehe.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wcuurjtd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ytsfbmnp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2cjhwppyz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2xsdfmrtn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2gaosmxxq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2bbyphrfj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2hhvainjj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2nhfauxlw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2slpwrszo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jihbypvv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2frkiawxs.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zhfaoctx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2viwdechd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2cmthdpbz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jbrmftvq.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2grvyguna.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2wfewojwg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2oqvcvvea.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dtwhllvo.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2csowbhhg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kkudprgi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2wcpjyasj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2izqkdewi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2agavsffq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2dmbxhaky.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2lcgwmltn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2aggowmfr.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2khgangza.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2cozfwfcb.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ryjnxkhg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2uwrfhxnl.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2uapaxqnn.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2lbnixywu.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2admvsbvo.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2lygwygvv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2quzbygxc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ogqqjewv.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2hpzbtzlt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2adjybqjf.html


<!-- 参考信息 -->