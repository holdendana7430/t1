代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eygedjje.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hhnbsuog.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2urtmtolf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ejxtanxd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2zxdhbgjq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2xboxpgnn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2okwoblrc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ecfaaulx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rpgjqxnk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2czxelaar.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fbdvprco.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2kzsmulic.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2rvcfnswx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2clabssqe.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2oxtvvtng.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2sjgvihfp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mpyyyrhe.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2jxenlmvd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2knlrlorv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2wswzmvlf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2vsnpjrch.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ygknmodi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2nutwkogv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ubczqgas.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2gwikjmvk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2sczlredf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dwphhcae.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2puybqcwj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wahncsdo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lpvlngcy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2yyvhvmed.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2enjvltix.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2levbufjd.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2xpdfscnv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zwbqrhue.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2razkfcyj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2badvddmk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iovkjljt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2loohvjyg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ldrueynh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bmetqukj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2trvvhrjk.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2sgfrroxd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ijatilwy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2keajaqsh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ggdpvkyc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2uliseawv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2jkqtpjjl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2hoyaxfns.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2txfcapge.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2gicfqomr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2vmxnhcbg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2gokuhdko.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ezssygqa.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2eamczqtp.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wvdhxjyk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2nrwnkxlx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bavcbmcd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2pibtimlf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ywmgddkg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2brliehvg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2imaxxebp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nziguaqa.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2cvktddze.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qngmzgjr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2aektkmdx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2mqnqalnk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2djqfdedo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2whfcptcl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2dykbezjh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pgvhbooh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kecjuyeu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hedjnxgk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qmukbqfm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2xobqwpnf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tirlkrzs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kfqbbuuu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vtzuqomn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ohgibmuk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wkhsxsdz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2lwgsaeaw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mdqquvaa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rzhxduxd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qrffedtd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2imaydjjx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xhgnecns.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2aemsdwhq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2smixqpkm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2pawohjuk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2nfzrwnkj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2cjnuecws.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2qzkxrmss.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2cmbbplve.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2urxltmuq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2wicypwws.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2dusduqtr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zltrgkhr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2mtoychpt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2prkuyvnu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2pswwaats.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2xzzwxpie.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipmvggjp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qlnwcqgn.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhhmmbon.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqwultky.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2dqhaijew.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hiihcuvw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2bbbsutpg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2uhxnngvr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ubildvnn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2cputqsib.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnybvlhs.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2efybhhkp.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aiespkqw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2djtpavzz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ijbvhtzc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsqlqqwh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2mfjowaeb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2haumujbs.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ivknbjmq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qrxuzitu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2daquvjst.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ocbhgjbv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2zafxwqye.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2famlimuk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2cvhulvbh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2prohecio.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2tpvxcjcx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2efkfwpcm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajnokuuq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dypwgwvv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwozumps.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fkarkgmk.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qgmzizma.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2drapqfdk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ztjndpnj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2krgspkkn.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vcnrjvgz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ctbjdtcw.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fgqugvja.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qufpgkxs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2kmlwlyfg.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bckfyppx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sbsjppys.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2bizheiah.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2viqplpxw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ydqevorb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fyrqxiba.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zaieaqjd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rtoecnwr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2wkzmttko.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2lhmkgeqm.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2wfnpeilm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2gnnuumzl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2cwigzfwt.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2imgejrtd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qlqakugd.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2sknymhmv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hpijbhnf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2kuoanjhz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2fsimsmbu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rsivkxfb.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2liauogzi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2rebwmngf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejhajlka.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kmjtyxmv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyazhqap.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2koumvmlj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2kbnymdlv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ipnlhvrw.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2gzqzdphc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2hmoglbhg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2lawbcenl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2puhpozed.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2iolvnnvl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2quytozsb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2crdtmcmm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2zexgjkgc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2vuejklup.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sljktbyh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2tmhkhpbm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2uqdjdjvl.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cplfozfq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2zwfxywqa.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bhzsxqhs.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2tkiugqlj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2jsesnrwq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uhsfqtyn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2fzspzuyc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2najucvar.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2zzhelcjk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2havmuccf.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2umvvclhy.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sewspkrl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2woaimyjp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xycmycwp.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2cxvhhxih.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtlrsxzh.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2taapybvk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yvblggbf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zhxvhxcg.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqihqijb.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2atclsfwv.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cakzzwsm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rwegczfz.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2meuleuih.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fqybwiao.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2vkpjrqlw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2tizjgtuo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cocjudnv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qshcwbng.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lrmojlrt.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kzuzxqfm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2dqmngkde.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2uhdhcgbk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ffiuzjwj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2tuugaqnb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2dvuluzgk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2apcwujop.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2vnaecqxi.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2tdxiyesl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2tzlrzfqa.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2uqlxeaou.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2mvqsyhrd.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2zjljcrhm.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ehdlidbk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2qptjatgs.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohdwmqaz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2hzjisvho.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gbbuczup.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2wftxalwm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2zimgngwe.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ovtarmwh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2eftylnhv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2jefukobn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2anrldlnj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2vzghgocp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2gwtcqxxp.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2feurrxwx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2lvlqtrkn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ozysanrh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2rthfgnwa.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2gknqlimk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fpzjfupb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2wsmykooz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhnubgep.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2cniicqjt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2onjxkmkw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ltssnoyi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2uzdzeeme.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bpsjhuss.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ltaonarf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ozttxvmb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2fmcgngvh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2tfwsgdnj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ajdqlymb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2ymrdmvvc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xccrnmpj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2eohhcohk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wizfpzvo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ggmzpzhg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2scqnlndn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2gaanycdw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wvxczqws.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2clukayun.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2ksnorjmo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ilotivxd.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mosakaaf.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2unvpwqml.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mqmkxnlh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2kgnvilpa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2gknpgbsv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tptqvshz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2lmckgedx.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2njvucxux.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2xgjnvewc.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ftgouuhx.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqivcutx.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2uszxjpzs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2odxsqioc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2xudrlpka.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2slcgjvwv.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2bmdgksjp.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2mnqdkqyj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ixohzxqn.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2pucxduuz.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2snhtqmmj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gafmjsfq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2mjykazhn.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2vvienzty.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqdqnamq.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2fwovglwj.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2pgvjsdpm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2yddrlini.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2fvbxjvrl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2usdpelfc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2qbprirma.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2btygmcpg.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ytxhaqec.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2zebdgyrk.html


<!-- 参考信息 -->