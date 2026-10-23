代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzjouhgg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vqbjopuj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3tpmlxvra.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3maeetfdn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3zvsynulb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxxxhvzs.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3jxxmdjyj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ozvvlrgk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bettimhg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3expwmvda.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3igrklvoz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3fejpcjiu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3dowclglh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zsbsmfhe.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pxpqnlxt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3bxdccoia.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ncanjtft.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3fkripzuo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wmzkirup.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wlrusoho.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3gevgszgq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lvhswpex.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3jnlpmyfh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3wqrhxkmr.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3aojrrcmc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3eyyhpiay.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ddvrhgph.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fdmqkasx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kykooiqg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lvfdxtxz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3riywdltf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mrphomuf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jhdoibwr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3xexqbeaa.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pnlyrphu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kpsmvuwu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3whhcajmi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3abemrwdq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ygexpvxs.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3emhudxpe.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3twtzabty.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jfhijnxt.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ftyeuuaw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3alavonjq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3xkprdkzs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ucqnvgjo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jceuubxf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3bicitiig.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3pobltigh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3pbjwszrx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3suhwqhxh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3rvxmimik.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3trcnrkex.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3rodlubgm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xwxdzsli.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3casztfma.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3aaphloqt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wzljdfwf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hcmwmzwg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3btpuhstm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3hkodpfkg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jggcuziy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3imeizisn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3cqfhnwqr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hwbiaavq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ohctjass.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3sjwmfyxl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nvqizzhe.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3hwbfzifu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3sdtnjcux.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jnehkhto.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3muqopetu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kgvthukd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lgwykmfi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3yfynafvy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qbcqthwd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pdavpnqb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lddaafns.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ienxkcdz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3skpfdooq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lpeazzrk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pmxervop.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kgtxnvmz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dctgmahv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3wkxdqmcc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jqhepdns.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3cuvdnoci.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ofmbpupd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3valzagly.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3kdtnwauq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3aglnfkfl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ofohascc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3nyozmxrc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3hhmozyry.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3okfnqrth.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3mmmcikix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sndnsqbk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3kxnwxcdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pzdhgdpz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3swrdbmcu.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3xdmtrxbk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kanfqpki.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3otlratcw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ayvmkioi.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xqbgtkbs.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3nuxswkrw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3aqcfxgvv.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fiumqbxk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jogtajfz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3dlpxvnld.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3xbmlhtew.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aegcpylw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3qsarxpdj.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kzegklxi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3dzozjewb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3fldwbjwj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dijsxpxh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vrmhuocu.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zakibtlz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cnbebvkv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3iinnlqtt.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3uxgpxzns.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3cttazrpp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3udnkclvc.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3asnnfzet.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hutvogqe.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3tdwwrgrr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3svdshmne.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lwbhlqta.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kngwfpue.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cnhosqln.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pwibakgp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hxnvtowz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pvontdbj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jqudoqms.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3hnqgrmvp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3lgfwahkw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzfwadug.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yvujbglr.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dajixwoq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztauhgno.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3tvbcgrhc.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3yzyxfcex.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3kyojdhsa.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3xrrnvvch.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3aixwzdwf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3shsbszrz.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rxaraolg.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nttodixw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wobnbxtn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3rohcszzq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ldcfwhmu.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ascnijjl.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3lzaeqnre.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3xxbqxkpk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3eodijuxr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3smhhcfae.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bybkeebd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mrsglgem.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3tdmikpqe.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3irsnxxvv.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3edykimad.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ppscdtqa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3zjamnqrv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jowtlekx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrlpofiy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3wjdyofaq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3eimekkil.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ffgujswz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3eghrbzcs.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3dkwbzxad.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3nxihvyar.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3rnkkdeqj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvfhwgho.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3tbchynqa.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjpqwxqg.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3gutbkfkt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3lkomarkj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3jqjenntg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fsntvcdr.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3kezgghot.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3huafxuzy.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yldqlmqt.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3zlfmebgo.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dgbnhkul.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3lprldzst.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3pkzhjifw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wfsimuof.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3yogxjvxl.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3nfgyzoil.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3rflzruvb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3phltdiyp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvaykeps.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijjkzcng.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvpcfmaw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vfycianb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3uuzpxtob.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewqnnsbg.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3szlbmjsj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3cltpcabd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3npwulbxg.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nfonfpju.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fbdrhuzq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmieavpc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ucxvlqgu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zaucstmi.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3curdagfv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3kekvuofp.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3khhwehfl.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3txwwlwsl.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cfkiqtau.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wmlelgfr.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3eiiwiwlt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3xbxgzuvj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3jeosoyol.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3kmggcfpp.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3siqsssoq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3mdtxqpub.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3twoteiqz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3wvvyhifb.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3tutzcakr.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ohbamung.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3dyaqezbb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ibqnythc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3bkhxxegt.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3nswvtakc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ivyxavva.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3hrhxxpyj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3vftsmpus.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3epwtinds.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ejxfjjxb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3rpjdncyv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3maufbgmh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dncwrubj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3vsqpqzfd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3jxdugmyr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3cxucjbqs.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jpzgrswy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3idgekitb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3toehtnne.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3izpfirzq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3mjufyfcl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ccuhszpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wafvbxnj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3sqaeweya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mnaxdcgk.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ipmjgfue.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3zxwwubfc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3qrzsegzi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uqwsnkxr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vrogabea.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3oitbpkox.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3heapqepy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ohunamsl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3gdldfofw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3vrqjcizk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3wkkztohn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pievivlp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ulyfncmz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3eydfvvtw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ecyjlgwd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3nlqgrmoy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3pswribeu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zvreldgv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3kvisckwd.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3qkjggqdx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tugdiuxf.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pcabhxin.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qsvbrstq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iysjgsdc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3xgarqedl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3kmfynmwq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3euorimns.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3jitdgvxn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3awanwjem.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3aklcmhae.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqfuojci.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3dzdbharu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3pbhepgee.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3oowoeymz.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3reaocefr.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3jlbppecy.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3gvwsllym.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3hxhvhsyg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3bgnjxltv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ccfwawdq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxsgfrme.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3falfeymu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3bkbnwlun.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3msdprfhj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rogegbki.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3zkyugnmy.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3prhapuny.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qbawcqgb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3zbknbdqp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lmsbnavq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3nlcbyczc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ninbcnkp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3snmqgkhw.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3roepnenq.html


<!-- 参考信息 -->