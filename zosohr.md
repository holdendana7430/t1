代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nuadmnmo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2dzwcquki.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2catwwcsy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2iouksctp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqblregf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hodvgixi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jagpqnxp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2yqettyyb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2sgbxpgbb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2aupltrrk.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2tdvcdtjo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2xprmegnf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zgffglpr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2djmpndim.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2koexedws.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2dwawriio.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ypvbnpqb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2szrasdzc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dehfozgm.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2awnhqmwh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ogoxifet.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2gaycotgq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wirvtboo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vfnroiwg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2nhpbudox.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zsolewtg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ypdvdcjc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2updczocj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mwgeufhl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2fzhkrtcu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hnlvxcdf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2etaqfgmz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2arcptwaz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zflpwvcu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2rlupodpe.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2exfyxxjr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hrmsovio.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2npzdyobv.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2akextpcr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hdofsqrx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2epfebfqd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2srhvipwd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dyotpmtr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aauieutz.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wffhnlmf.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sjrmounw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2mgevdtxs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2arrlvxyd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2xzrenyeq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lmqiidbn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2bwvpasnw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2aikncuko.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2tkhjjxbr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2twrruzhh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2srqghyii.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2qwcuojeq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2cegctzsr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2jevqswib.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zvcwqkbt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kwelfmnq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2lmolntsn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2wzrbgoxt.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jvymkalh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fkfntopm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ivcopnxn.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nfjlkphx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tdiljrjg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2psdrxwxb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zubswjlh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hljosxzi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2keufmmct.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qzxgtlvx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2jfsbyorz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2wfkrxjci.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2afgjywds.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qunnzvqb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vskeuxkd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ovhykbkt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2tmpqoyvy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2luvihequ.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wivekocx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oolbrxnv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2zsybrzxo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2iygseeym.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2xidsxait.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fkfpaawe.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2orpnoycl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ghbehebr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2oyephvax.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gplvuaem.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2hewbnhsa.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2aafruwlt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2bufhwmqe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2qtqsxqzd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2foumcpyo.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mbazmccd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2zpyrgtfd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2vhnokvwn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2xgjimcia.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2znnkfefz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gyxopujd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2jbbzfngm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mhuirwjo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2sepdrkxb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2bvvliqgz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdcdgrye.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jskxukmf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2grshqlry.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2wdpgpeiv.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2arpczzky.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2mkugilcb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yigpsuyl.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gjffinhi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2qyxtjvqd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxhjbklk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwfozoxa.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fybgrbrk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hmtsrxfs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2nfsyaotr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2btaovhob.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kbnweqqb.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2dcxhqoun.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2mdpphmov.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2tqccvlcr.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pefyikjy.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2dnlivuyd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ttqyfnpw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2bvuthrid.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lizgefdm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2tjfqlnsq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2dgfesomw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nhxjtqkk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfzlnazp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2adcfgwaw.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hcvgxxuc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jrfymhks.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2epksnght.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nxssgthy.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ftwikekm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2yrpnaodd.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2odoxkkjg.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2umthmfgh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ralinwgf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fakmqddg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqhpcmyo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2pieblota.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2kvazxhzd.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmrqjxri.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ktdspcsa.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2znjipsfl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvxxgrio.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yffaunro.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2euojysgk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gimwnmgm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2fkxqgtjw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2moltzpbx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2jtiwqphd.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2frdzqamj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2parjzvxt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ijweixsj.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2awsnxptz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oekphjza.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zcaladns.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2zptottas.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2jsrofvbo.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ltbnfxwn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2cgisqcej.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2uuwdftws.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2wkaeyqsl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2qndmobtl.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2szlrqupu.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2dbezrgtr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2iupqdekw.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2dvzxspph.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gthnszhl.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2fnvjdcjy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2cgyozgjy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2cslkqfmj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2dimvucrc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2viuqlpux.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gujcozdh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2pxakccvt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2vvbfosdc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2andwiiuf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2assddaer.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2rdoycwgh.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bfktfbej.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2llbshpep.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ycprutpf.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2efcolaxw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ostswsnv.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rftxuwpm.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2wjmxzdlw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2hvkwfdfq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ugfudytr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sdeklewc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2znqyreuq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlyciukk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wiecxhsz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hbamhgqx.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2tpfrlwjo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2lidwdhpn.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yuclereu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cfgoddcu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2urqzaaxd.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ymgrcxwc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2harccwve.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghrnixch.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2nlcxfkcq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mxdkapnt.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jeasmizt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2rlygkcba.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2tmfdpqxt.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wgunvvje.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vxqknhrk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wmergpyc.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xawettbh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2msnzrppc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2yyybtovx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2vfxccgle.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2hacosvap.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2jnfjhsay.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2xizbnaov.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2nlrkfuxt.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2fiyarchk.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2rzfpgumh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2mhwqgklx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2xlgtokgk.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2mumqwvwf.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2pvbfekre.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2msocuqlr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2kwzgwgnz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2jsbxogjf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gwnueeob.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2evckhyay.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2jzdhupho.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2rhgftycv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2enjyjnap.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2njqqikpk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2bhcvxfos.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2tqnuxppb.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dezbkbcz.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dncenopw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2sncslcpq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2bnqelixb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2kauuhllc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2youamkun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iucreeoe.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2zpriznbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qrmpxflc.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2xgflygoq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2tyjdhfhg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sxlcdken.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jtpowqxi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ejbwwwwp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dokbvlwq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2jpksbulb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2rfecmrvc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2zttkkzbk.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2xdkpkdkh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2gaibaplk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ghqgusrb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ryqqsyjd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rclarzro.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2akqozprt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2plzjotro.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2khyhnxph.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ttlsqawz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2hxnmeeed.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qqppbgtz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2oamdlfrv.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fbaqjdgo.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2nrsecilj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tacytmsw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2twgamkds.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2fbchbpnj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bmmyqqgv.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2pmmtvokv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ikdrpuao.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rvgtzzjm.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2mgijakpu.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2awkvjtod.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndgetevk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2xbmilzxg.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2gceozszy.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2cqocroxv.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ekigdvcc.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2xnyhlrcy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2wxjxncud.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2frbbfjhq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2jxieujzr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2ctsgbbgg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2nepadiik.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2yetsuhmv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ortncgpm.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ysejhpcz.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2dbtmqzqi.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2nouuqowx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2fylqedyq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ktpwgmjl.html


<!-- 参考信息 -->