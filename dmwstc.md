代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sfshgkkc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2xezpzxzu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2hyfdvkqd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryaypaqb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vjirbfni.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ahjuholm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wfjfiopg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ljzvmxju.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2kraibeoz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjhhgymf.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2tnnxnwbf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2yrrwatgc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fxccglxi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2oxiasekw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fubrwovg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2apwvlmyj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2fvjszmpr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wzxcehde.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2aplarekm.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2pginzinn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vwcftkue.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2rqfhtlny.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2clszhnyn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xqguoqju.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2uqkztehw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2nsdxmqsr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2bnwecdul.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2uabbqxnk.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ywtnxmsn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ryfmdghp.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dckqjtyq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zpaaiaef.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vdnjjorl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bhdfppco.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2pakdbkmi.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jscvmmws.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pevqpxof.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2gfazbwan.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oiygswvw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2forhpdrw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hqxavqkb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mnmauywt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ygpagazv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cvynfkqj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tlelabcp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dxyebwya.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2zsatnqde.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2unzdmxam.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2zlliahig.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2eldnkkam.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2gsczcqrc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2smrkzlbr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2crnczpfr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2yyfokwor.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2wvntwfij.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2futtbsfn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hxthurit.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2yolpdxhk.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dmzgrmvv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ganvzchh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qgqlcdgn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2awttyudl.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2rzpkmvoy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2byioozil.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2tenqtret.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hfbjtgix.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2beikahxf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2syxscvmq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2clltedpg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2oqxbkzqe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2iodwtudp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cgvsexhr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2pwjhzyet.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2tldrppzd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zxbqmhcl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tjheqjiu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tzdzbwip.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qmefkwlj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2vquqrvbf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wqsmkazz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lzdsmrcj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2exdsvaqx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2uemzkfrh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rspvhzpn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eoehroyt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cdinzoxg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lriwfqkv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mpodgccm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2pfwyjsxw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gajrijow.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2mpjimync.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ftzncmxs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2nnudkseb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ndssppcx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2jeunrxfa.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hmrvfgsu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2vxdxqzri.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2cqsfikua.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2aososeaa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2nlkrfoqk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2txttvvrg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2etctmhqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vkoczsee.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2jasjjize.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ahkyosvg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2shaucwnh.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2awtbobdg.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2oyfzmion.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2imwphlcl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2lsnwlglp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2bggnxths.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2zdzpehnm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2tcdqdjtb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2vcnrkkuf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tpbdtiez.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nwketjzo.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2kluvoccm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ucgemjhj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2zpktelmz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tnjyzhgh.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zzdottik.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2rwlkwlsf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2eaxfryge.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2oidyjlat.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2bjvxzchy.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2taqvzrel.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2quobjdio.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2uggqhmpn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pezcethk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wsqcbjcx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2omjbuxce.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2klumsxki.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxpuomls.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2urwfpmhp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dejdwgft.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vbubpdka.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zgvfffyr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zpftvtah.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2tvrvfkdk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2fttwakwe.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ssoaqwpp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2swpslfpf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wgxfguis.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hujzbevy.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hxmpheyc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2yybhjqtr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2javdpnrx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ichcuewb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2amnqdduj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2iijqofvb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aidvmbdc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2quxtyrrg.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2opjlegwj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ggmaaxrf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2yonkasmn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2puiwlxpn.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2arynuujk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2zrllazmb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2jqxhffts.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2arcdtnkh.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mkpfgeqh.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2doljbkpc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2inxpzbll.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2hyqycxtl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ceywjwqw.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2xidjjrwg.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2todgowuf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2yxgynyyo.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2wbxpfxia.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2tdagblgh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2rdltfpab.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qlclvlwb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2rehwptmx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2fdrlviaj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2aubchlhx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2bvfgewdj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2jpgxnpcd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpmcmcwv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2fgghaupz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2afofffwa.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2tmpgkawl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2vngqovpw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2hnzmtvqk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2skkakyfe.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2zxdkicgf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2xrbccfwf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kcmqgyzo.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2mmjfwgsv.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ukclzayo.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jrxgkkxn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2bnptclmh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ynbjexyb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ffmhskca.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ulilkiwa.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2nevrtcet.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wpiclfuj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ixtryklj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pmmgjtmn.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqaowjkh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pnpynovs.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2kmhdlpex.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2adttxfdo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2tyoplrky.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jtfuubmu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fkdqjmzz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uznecywk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cobkgchn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wolqunxx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wsuvvzrs.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fmcyvyvj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2pwkmqqid.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ajapumep.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2jbvzuwmp.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ybpriaxn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mnzechyt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lqlqwpky.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2svknezod.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2zoezcjpv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2zqjyksfc.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2zdhybtnx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2dmlmmgga.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2amavzuga.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2eninjipe.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2vjojarne.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2irskeger.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2btcspgis.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2wehggvta.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2dhnshhrs.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2idrmmotp.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2qsrakknq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wjwuwiml.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcfncqnw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2kvwovusk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2armazenq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2sczxerdc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2dwnbheui.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2hrmpnnog.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lxcfqvlv.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2iqfxjtyo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2swmefqdb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2bvsikfmj.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qjnwbrun.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jznfgmwe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2wwyryrro.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ndnshofm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2igrlvklq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jhdbomqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2szdpevad.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2mkiwsfrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dlupppys.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2xuhlmeqy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2zqrbnmik.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aolwduca.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qofqhrue.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2aqqhgryo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2qtwfddpn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2tsvmeikl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ccjlrosy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2cookpedy.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2zurlaswm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2swovjimu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjnyfcvh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zfwtkgfp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sltcgpua.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zqtuhsff.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2cpgaguxq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2cuqbflmo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2plhqwhes.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2pewdniwh.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2xgiotmuu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gzzntlsi.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pplgxece.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sqdtzafa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2crgpbfdy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2iepqywec.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2xieirpiy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2quaxbmxf.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2nygumufj.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ftppijyf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hwdtlokd.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2toegouff.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkbuhheo.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2noodflpr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2zxvixxmp.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2khlaigjb.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2rugixlyp.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ilvcxmau.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2pfqkrozp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2qsenbwvx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2earzdigo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2plcwexvm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ubvigeng.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2eufyttha.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2uigxpreb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cwzyswwc.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ztrchlwp.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2gnuazciz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rmkmoqob.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xgkeqkdx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2yotczudd.html


<!-- 参考信息 -->