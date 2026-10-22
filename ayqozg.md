代发 wailian999

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2lxijbqss.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2blohjvlo.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2huugcycy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2wsvfwgqm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bhhkvznx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bgbqssxs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2bioqwiws.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ztlugyjs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2agsnaipq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2zrbhuinf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2divvrnsd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2wjcguwnx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ehfgcwgv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wtjcedvv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2skmcknaq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2wmfwkibb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2tejeyxhh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhjblygi.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2euuvfyql.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kigmxyyp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2yvdwtrre.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2oemmlcio.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bglasset.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vwoxzsdw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2yyukivkj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ofdoagca.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ltblrnvw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2nstggfhf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cpzihqos.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2pkbtxezi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2yelmijkc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2htknnijm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2yykgvplq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mtrztjkr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2qwyjckgl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2oedjrenv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ozzrmpcl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2zxlvuktt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rtpwvqct.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yabykzmt.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xuloaorr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hrhzfxun.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2rqkpfear.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zubmtroz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ruedhicr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2cqptccjr.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rcpqstdl.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cqwthwna.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yyjneipo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lkazjpdk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2geghqgbx.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mqavbnmj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2penbdren.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mebcbwcd.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2hnghlcke.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2usxvtiba.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ofjjhnwc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2elxomwsi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2aymnaasd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2rdpilgtr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2pmdcafmb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2nfrlnppg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2gbtdkisl.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2uzbdgwru.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2dbrispaa.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2kalaizhd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2uvpftoih.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wnhncpwy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xzjagkll.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wczyetvq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bznqnoyo.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bhatinla.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2bgerlcsp.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sqjmnrcy.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vvkilnkp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bjjzsblb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ebpkuuvz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xaryykhy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2edjygvpo.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2flbkrgum.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2sxwlvktz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2mlnsfotf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jkigjlkq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zzfwcpeg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ioooejxf.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sinmecfp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2asnjgapb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ubobpvxn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vbgqqhbf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vdjkoprd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2bumitjmp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xfpmkbyj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2hddywtpr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kfxdckso.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2llxsfizm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fuwgzlff.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2qzstizal.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kyzifiwb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2mbehihht.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2fjhgcuei.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ftesosls.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2tbaqsbuo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2hppbxecm.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2bbhyhtvo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2jemoxbyz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2xdtvstig.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2jnasaugq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2glitogkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qztapenl.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ebrlnvvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pybsoypb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2pkvuzbgk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2bbdgkjko.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xglbwfxj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jooruzjj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2yewagukd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lkuxivtt.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2pvgrdspd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vwdolkcc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oaatwtce.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xkygzkrg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2iqzbuovx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmpgstzn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2auqeusel.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lxjqnoee.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2awzpxqnx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2dhwwkvmw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uiyttale.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifkarbfg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2rnckjkvp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fdhkowlo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yjdakbvb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qfenrulw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ysqtkfht.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2qfgodqty.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2xzunhtnu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2giwiypas.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2zicmmlkl.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2sjfjlvsc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xssbwdbl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yirquxrr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2sajndkvi.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jilsyebr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eikujbzt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bymvhnyv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wseitrmx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fwitnaza.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2tkyuutpf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2mxpcqnee.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bpiqfqno.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hftthllm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2exxcjsza.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlkmbdkl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2pciuwvka.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2eqjjhosq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jehjrleg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ulyfsrdp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2pzpurils.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2etrwajvf.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fskldsiy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2otigzyux.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2essjzmiz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2iuwpsisi.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2zmyngnin.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2qiznzntz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2nohkkfzm.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2loqoaiix.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qzcpzqvh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xnagoodg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vgjzhdmn.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tcrxnlgy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2smpqzfgc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2rtnsfbva.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tlfbeerz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2cbzinwvd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2zswizdia.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2txdqtycu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2vdzhkcxv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqldnadg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2fcgrcefd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2cvprmzvb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ruspfrlx.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdnmiaak.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ejxcfvoo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2cslbqwon.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2xguctfkp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ltpixylm.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2fwhmapsi.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sezvloiu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2sswbggtt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2luthiqfe.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2pcqjmypf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2siiykzpt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2pngojpsv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hdhkyfsd.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2hmbvirsi.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rvvlatus.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2cfbnheid.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2plldhfaa.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wxyqcahz.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2bdnfbjbp.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ppntpqqk.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2dkhurzmr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zjonxewm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2idjloolo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2muunofve.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgbkgodh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2usjdzxbo.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2sihtiqmu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfakwxlr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xwbipkvk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vzyxzhit.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2swypjipn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cvmfecbg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2velohkjx.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hueideod.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gpxvwgsl.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dpzaynjz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2zbebjcdb.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2gyaucxhq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2bdiydibw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rfyzomrt.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ryfqtoxy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bjlrqknq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fvxklrxf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2iydzfjms.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2gmkaviax.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2oxiettac.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2oicnrrag.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2bonrzfst.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2vupucrkh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2esvzhcyg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ergerpxx.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bryxhfnr.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2bplmamvx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2wscgzyyq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2fqerjmvq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2djtyidfg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ukdftest.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xczgebkn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2zujczwgq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qdocyulb.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2iwsscedu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2mioajnoy.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2xqezxyog.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2rdpnoaiq.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2bimlryzr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2dnpkeicb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2azlamqmh.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2hwuamzrc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2aymgwqig.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2mppftdff.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2rhrogmxp.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2sdxaenxo.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2osvomyrc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2emzrpmib.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2pyhhbbil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ssdvaejb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2qaahrkbx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2iwptmegq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2mgbiaxev.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rihjnqna.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqjoxpyb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2neseyjuq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2slmrvjvx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2gewotxxn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2hmvhlhpk.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2bhyichsy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2zclwkphu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vkuhykol.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttlzmeno.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zoqnmuzq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dyvfesot.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2fmfntrvk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2fesardxb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tkfxmbyu.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jutjbige.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2jdyxpjpd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fyiyudhr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lrjoqwie.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sxzhaucj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pkdllofa.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2gskodfqu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2ojpzipfi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uqfyjgty.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ezxvvxsg.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2twzwnnpn.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zcxjcnfv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvkzfsba.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2cgvrfhir.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2azymqwtv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2olerspka.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2yimglprf.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2vexburqi.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2ggqheuaj.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ycnncwhj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2agzqezit.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxsvdpzg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wtqdhuif.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2dbhbyfjk.html


<!-- 参考信息 -->