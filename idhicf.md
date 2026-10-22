代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2tkizofir.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2karsrwtn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kacsqhxk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2clyutwka.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2wgdtifmq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2hqmmgsay.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2vzjpffbo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2mtzfecrq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2crajytae.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cciqwadi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2agzewqwj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2umxpkpyr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2qanlosye.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ljhjgvrb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qwfcnwew.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2hpwmxsqo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2btrawajb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2zybuzsvp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vcatjzpj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wjienfhu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2teefxbjp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vtirtsrp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2wnmvtswc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2tbjeyojg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qmfbrfpz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2qqlbgvqr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kfsihtby.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ctbuphky.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pyvgqled.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wbnnuscq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2atsxvpec.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2stlsapkc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pqfdnots.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2gmuusthx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tnwmfqcb.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2elyqwnjd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tubwicmk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eotjlfss.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jdcnqwbs.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hpoonoda.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bdontnpo.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2igcumycf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2uigpmflp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hyuuydlv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2dluommbl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bcsazsod.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2drdppkqg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2onnyinal.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2cywlrsuy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2sbdwiygr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2piuljpfp.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2edxotkwj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2xantljiw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkqonuyr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wlbthzly.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ilpmocjf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vvmombpa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2xsvyhzuw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dvqjpkim.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tdsuofxh.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2qsbnsjti.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nketfcfh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tjidusjp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tynxzukh.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2isoyqdbj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wzsvssja.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2dfnwrrke.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ftvwidbu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2svwjdkba.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2nnpdlevg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uguanqgs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ykwefwoa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lnokvjts.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zcxchjkv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2fprtumme.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2okoribuu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mgqkuhqk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2krhshabh.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2exvwhjjx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qftmvmuk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2oaqkzkxe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jijjpotn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cejmkzun.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xpkxtzzk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2kvgrrwpj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aqqfwbrd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2mfwppcrz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2aabamqaa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2pcyraczf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ywhnirrc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2qkerdmrj.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2gkvkhltl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2vospydjx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2akmzeusw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2fuljfszu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ahukpqnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kxywrpwf.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2cpcojbuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hwfbpaxq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2wnxecrel.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2payezxjb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2jvvojvqw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2tqrisncl.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2foyfuwoe.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vicvscgd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2nfokhald.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ayxcctdi.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wxgjwywt.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qveyhicm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2iijecdbv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxrcwsoy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bduqelmb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2abrxmkui.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pavmabyb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2fdwbxtpq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2dglvcfdq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsvkbxhx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2kagotivq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rhsfliwn.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jjckwzie.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dqmjxrik.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2vvsbmwgj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2aqxaxppe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2bolimdsg.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rutfaovv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xtwpekea.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2dharuwtd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zxkqcbej.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2melfqhwr.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjvvragj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pbnztcqg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bjcsjpgh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2umpydaxi.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2svbhsvha.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ahoendbb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2gnqfntjh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ikmzwfic.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cxenejsy.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndkeizmn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2plzbefqk.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vcgpbglw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2txmickxo.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2utwzmjqe.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2upnigdkd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ognekrmz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2thgtmxoz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygfcevgt.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtajmihu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cshtpiwq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ydwpvlbz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2xfstjorv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2zbgngjhw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2jijqysjr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2fbulswqx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2goshrpjr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2opqbvwag.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ddblwppo.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qwuhboob.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eldlmgwy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2wlckegft.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2sgeatcxq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2npultvgf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2hxqzapcr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2oaxifkeu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2xspenhkf.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rmiesnta.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkvmpwhm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tzziilxp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2lmiqrruu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2bfwxjziy.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilgfdsrp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2hxcvuioa.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2olzrakvb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbshloyy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2mjpnnuis.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2rcvldknp.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2behameve.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ujrfhcrd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2sfdowiwk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2lypacfsy.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2lyrnyoxi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2uqtvfvhu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2svkyphal.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2dixrlwfm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zuobhzfr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2mojndvpl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ybajhvlt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vkgfcshm.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2wxbjjixp.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2iezqrjli.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2arwdohnx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2imkeudal.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rhmidcva.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ntyxdpzt.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpuvunlq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2brpukxzq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2clrzexbk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2dicrrzff.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zgvrpyop.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rsoezboh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2faqvilux.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixkzsssw.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tbrfathm.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cplijqdc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2shexqhwp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cnrhzqpp.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2akxbxjkm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2jhsszyke.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2affiynoz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rkqdhtaf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2barsbqor.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vrhhaqqi.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2izofqtqi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2qsugrvhx.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2tplbpinm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2qamotuch.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2jhadnhgo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2fjrmyeln.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2nfplkqyt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2rfmcnjqq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2shrvfpnv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2jjmlhopf.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2apbxjmth.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2viqunldh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2xzbowxhz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2mczqmsao.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2uiggpxbg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjbudwnk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2keubqvjj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2njomynsk.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2vsfvypgv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2vqpqsdul.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ahbowkyp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2tlqqigxm.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2nhfysdpy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2uewvatbj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2qnvlywvv.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rtstqfir.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2sigymyng.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2gihmigmq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2whdevtfw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2huygrcbs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2qnbdjznb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kttapcgq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2iohimqya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bovacfem.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2wemxgknb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ryotoang.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivivugtt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqzypzhd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2wycxuled.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2gqlomtrz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2ysjryjui.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2fnoxafnx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2vavfhbff.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2xurxgucr.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2tkghrdys.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yodctcbw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zqukzfcd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qmlhhllk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ebvvxbjf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2njuwkxjb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2bvqyxykd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ludzpwyq.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2vekhgvvm.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2zfysroix.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2eewxbmeq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vasdhwqn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kbdxmsas.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hicftuig.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2fjdgaqzn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2pbqvlotu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qmshuugn.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2hypurffo.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2yihidojx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2kssnkjfe.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2smhejdgu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2uixjkavr.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2cfgniviu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2hrkjsloh.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2lybxrujw.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2bxsafqoc.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2gcimteml.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ofrevpxm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2orcautnp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wctstqjr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2apuvnnec.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2cqdihzsv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2nsyacjxb.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2tvbgxqib.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvyxtwax.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2gnyzbjxq.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ircncmbv.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2dchoebpc.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2fulmtuun.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2vewrrwbg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2liaiatot.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2cnbfasgb.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2bygsrwqy.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2nvtatzrj.html


<!-- 参考信息 -->