代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3quxvkvch.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3qfnzucye.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3amklfiho.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3tyjweyfz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ysgmdlth.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3btoaollp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3swytisgi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3htedijni.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3vxqiwcwp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3tzflokvy.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3cbwtsoro.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3lxlfacnf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uvxzioln.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3umhnmbgs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hgnrqhbq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zfkbtaod.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ccazvubh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3khaxbihm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zikjmywx.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3mlpilnqw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xocxenos.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3hopmsifj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3masicjgo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3widkycol.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3xlpwmwxv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gcjwdlsk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3maewuogi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hwyupbqb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ahwzkfjj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ykwuuiar.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uchujgqx.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tefowvae.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3einoopik.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kmphwttm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3hcbyzckq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3robjouio.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sbbseolm.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3cscxojec.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3whlbsxxp.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qwkoycis.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jxnjcyej.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3npivwrpo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rrnhmfju.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3acruakoc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3psydkswc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mtirnvzv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3incybdoq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xsvyvjip.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kcucudpo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3yjwjjavb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3oiubwhxh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3xnxvkpja.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3lhndehze.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3euhbdfoe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3zgvdlfnd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3gvzvngzc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3qlooifan.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfwibukt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zcdqsxvg.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3skhiwohv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jflkyemf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wsrmshxq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nwqtvler.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oebdmepe.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3myljnjcn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pqsxppse.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mujtpffw.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jpsrshll.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3sxrmppir.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yhagebol.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3mbsintok.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nxkhhulm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3cxhdywng.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3vvpmnqnv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rdlbsbcg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ltchuiwl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pxjeoxek.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zvtfnmwz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3gsdrkfeu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zpnpyzzn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3frnamquw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fgouqyix.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3vhgiozdh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qlltyxxh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wmlnbvbr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3aavhcbcd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3owvrzuia.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ccjsfiqh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3qszadphu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uuvcmbtr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ieuukasr.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3qmhgzkdb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3jsqewusy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ptcvgmad.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3gbmxrfbd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ssdpyntn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3wkeihrif.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3igzvwenb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3knfzptvw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3okdrbwln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kicjzpxx.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3iagedrak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vxtwylto.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3pnqaothd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ilthognh.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3wbxcjacn.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yuwbnojx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3wmpqhfkx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3bmskvprk.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3pxwcmjju.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3gzktxrwz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3uiedkcey.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3bdnjkyac.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3zdkalvah.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3gguqjmuj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ewkzskmm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3mlpvatxv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfubhupv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3etbjkiit.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fxwdamqy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xfngsvih.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3wkpapbff.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3osamlwhw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3naegmhdd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3rsrcbwgl.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ddzmqkex.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3bdximafz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3xmoqmfla.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lzgtksih.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ztrauxrk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3phvkzavm.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3njcwdnbl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dujzsktk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yseadqwb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bynkyoin.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3simrztbh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cqxozdrz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ecstfcnx.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fudbyanz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3wpqspkod.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3uhvsxyfq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jangnzei.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sckdozrq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dbkxveek.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvrqfjfb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3mmndlzgq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3dzirqdkv.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gdcxwbdv.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3cwjvefxb.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3csnzlpmg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ettgdfxq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zipyrrsx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cghjkkfd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3odmugiav.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3wukrodug.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3vosrdouz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3mwozyxwe.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3prsrasqq.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3rhrkjnrw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3abqpfirb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3prrampmf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lacrramt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3catbelyo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3djvefgzp.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3nucluvne.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3oersqevh.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3uhviqcmv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3iexmbfrk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kdxqpnrl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwrkrhue.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3uvznypvw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vpkynjrm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3otmojyyr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3cxmwheqt.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ctfmphqn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3hsswyxtu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3djdmxppy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3kquyiiic.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3iunlfwjx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3amlmxclz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3faobjohv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3tjshyxkc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3kvmbalgf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujibrxww.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ldgjqroh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3gubewyiu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ijhxjeqc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3dnmkarju.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jdruuwwg.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3nrpbiapp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3qnsfruiq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tkukasnn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3wwxhwvdv.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3cdgxgvdx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3smvcdnsa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zuiqvwny.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbezbcyd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuavqjrq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3olgkxmxp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hgyctxlc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3kbbgkwsl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3hjrcntes.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3skyskwyw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3yzslnwjp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ykmkreqf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wlqmabyr.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3naucyldr.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mxgqghgb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qarfinsi.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3cfhudlhw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ekdqwqca.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3cllwfqyb.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3fncneqxk.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ipqpxzwg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3enidudii.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3iyzquutd.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zvuasztj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3nfwolyag.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3hbmrbykg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ldtrkhoj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3lfinerdu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3brfhhpdc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3owgerwsf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3idskzios.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3evhhitcm.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3asrehofw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3jitueyst.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3rzxpkumx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3kovtvgvk.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3wriduiqq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3yxzuxehg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3azbepuhf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3kzkuybud.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hvrypbjk.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3gojjdinr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3jredoodg.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3jlafacur.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wdcnguhc.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ofommcgr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ixurgjgj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3anhyvovc.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xgoludrg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sexyeyns.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3bkwapbrp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3odobycox.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3qjeymekp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3rycyudvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ldkcyrxf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3dzssgtcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3npiateeb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3qjfovfow.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3uwzdyrxf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3psebgfld.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qharobnl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3jxhuixqx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jlhmfdgr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3qacjhrre.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ljypxezn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3wzvfotqn.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3rybyajql.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3himkebfg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zijnfvht.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3awpeskea.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3eidppfhp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3umvczcvp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3iuvwmklx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3xpucpefe.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aqpdxnvp.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3bjqxccqr.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3llnlwpiq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lmgascto.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wvpiehhf.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gsytswmd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ndpuwguu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3cbhzktxa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3nzoyaagd.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rqlvdgap.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3nuszzrnc.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ygfmxreg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ummuajbs.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3yndksuft.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3wdkfmjam.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3drwgyvxn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3avcjxpsc.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3oyjergkr.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3rqauxwsq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3frntysqp.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3kpcslswg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3srfmswut.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lxcdgdku.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3nvpnnaae.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3rwrjeveq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3lxxfyfet.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3opvodhqe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3fcvjtbno.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3fluoypkt.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3qgipmnro.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3mhdecfxz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3blftrzgw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3rybblkyl.html


<!-- 参考信息 -->