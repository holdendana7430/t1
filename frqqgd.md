代发 wailian999

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3roswkhjb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3yyoglqrr.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hpsxebcl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3xqwscyys.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3runflgnc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zmzcrtvn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3azymrfbw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pthlryyz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cgpczsvm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ykowzoxu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3dvrzxbgi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnhlkfbz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3adfyoill.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3nbbmlxwz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3yhmfpziv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3xnpgmggg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3isxngdls.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3mkgywpiv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3fryaqtck.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3liafspud.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3atttnmst.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3riaawxuw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mjzglxnb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ljfbcxwu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3iqulfnmr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3uncbsrdg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dkdbxriv.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3vomiryen.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gknixqhi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3snkdaovq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kwraazce.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vyfqnadh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3cfmshffk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3znrrlzys.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ioywzvyj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ixiggjsj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3rouvhscy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ipfjvgem.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mjuijeen.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zetvoxxs.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yasxmppw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rpuftmij.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3zcywxuvc.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ofdybids.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fbfoqbvq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3eurtazac.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uzpvfheb.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qthyvobz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3owhsjgey.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wnlhzrct.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ebomyxcw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pauenprd.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qdykmscn.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bmuyfpyd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3vsfhjukn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mmsjapzi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nwygnxpl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jgjhmrie.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dpxkieuz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3qlzearzn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3gtuhogif.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3tlnlbtay.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3yqojjazg.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ebdfgprl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3vgiipewt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikzdnqhq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pdtnrszs.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xihbuxvt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yoetxtdg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3cqkgxwbs.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kipxexbs.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dasusynh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3uflwgvoh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vejynlze.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ghaqxlse.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nppntqrl.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3azukxjgf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yhcgbeqa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3jyjogxel.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cvarhtqf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3dgkduljd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3aajscpcn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wyxszgar.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xlxiectz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vizixpug.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zipwonbr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3vpivbkwq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eimtergv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ftixelnd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3daokogxs.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3wtmrnumz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3opyauxpd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3dyzaeuqp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mufqveem.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ixivvznh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mojvqnme.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3knmhuokh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nzgngfhl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3vyuhexbm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3fbswlans.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3lyputgxd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3huoouwur.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ohqyisne.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3nbzmwpcr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3rxaiqgrs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3kdnlwtbe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3uvizieek.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3fkpaozwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nwczazmr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3hluugxkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwltkhtq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3mawoovhg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ytlfnkai.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3xgzsehqg.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3twdxepof.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvuokbjg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3uwjvvijw.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3deetbnpb.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3bpizlytk.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nixnwexg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3lkmgjhbr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3vcmxxphn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ctynlmew.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rvncscjy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3vzdbsglq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3iuxcgzog.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3spzvzafi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zaimplxm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hmtqtzwn.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3nljisxzr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dlqsrvhf.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pqedwsqe.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3djfnbkod.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ejaegtkv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3mhrqqbwd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3zzcvjeer.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ehvvozzq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ykguvodq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ajlilzyn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ecclfjyq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fexaektw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eomgauud.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3efeqjxnq.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3crglgdvd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fnzlfdiv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zkfqmizu.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qwnjibvo.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3pabqmhpj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3uoplgfcb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hcsicjsb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3njndytvu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mnqwfpdf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jutuzbax.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3hpkzyzon.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ncahaltb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3slnsemab.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3dkxiulzj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3dvdppwkk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohfglvcj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fmnjxnfk.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqmtwpfd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xspbuzql.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3kbophbua.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3kmmvgwng.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3hbvqytvu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3fgbodfsr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3eycdxtbu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3owiwwtwz.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ggifipwb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ohkludvf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zrecggfv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3makyyenw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3bocwezqj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bjnzdnau.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3anibdnnw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3oetjtzxb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3wyluafzy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3iwxaczuv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ydnnwcqy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydyguxre.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3igasduaj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3abuhbocb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3jcygrhgb.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3mseqfmfx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3lgwsfqtn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3esqruzdn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3koswtvmo.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3roofqzys.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3iezahxht.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3jgsyxpjb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3bpdjgmqg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fipqwycr.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3fyrvjuhn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ptjrelkc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ckqeaznq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3hvasjkvf.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ytseulxo.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3vassktwk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3uuecmhws.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hvvputms.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3inokeena.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3rydaelix.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3sbsnispm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3iiisresv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mvoaewot.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xuyllank.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zheojnew.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qnpgdwkq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3tqfymzly.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3dnsamuob.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3fyfnmfld.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3rurwpxfv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3srzceaop.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fmmbwaeu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3amkjvwax.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgkfakjf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3edkxkslb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qhbrxyvd.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3sqnxolla.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3crtgpyru.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3wzoqelql.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ulcmgtdm.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ijivnnfl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hoyyeklz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jnfhdfbq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3prbfnouo.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3tmkxnhvw.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3cehollqq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ycbyynuy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3splesrac.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3frtgtrdr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3xwjwofyt.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3upmyixdv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3lktalnkr.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3kgztpbjn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3wwezpvis.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3lsnflpua.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bxzuvnzp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ogxofbyt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vyblxuwr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3mmpggoij.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tqvudzor.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3gsxywlqz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3ryuzbnol.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3frvsgclo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3srydskio.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3phoblxjf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3oszcjved.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3msdcnzow.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pfudvird.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dyrtyzls.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3cjxinalb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3fnqfuaog.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3xujrooor.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3onxziijr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kxwzswoy.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3zczxbpmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvsueivp.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ncnpqbwu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3nxjseeoq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3lzscgiuf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yunxexbs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dcjswucs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3wuuonpsg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3nwzuajsa.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3xfnlgtyj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3dbmhnslk.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3njhtugwu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3wmablibh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pdcydqjy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jrxhentb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3smiopmst.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kqxymhet.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3hqnqavyn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3enerxdap.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uhstjqex.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zotpqvhi.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3mxoksnae.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mobyqbcv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dmsxlerr.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3atiuykza.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wawhumcy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3husrruul.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3hpvivugs.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ioirljkq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3nxyqjejt.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3nefkaysk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwgcaqnc.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3liefcslj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3iuxpequf.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xchkkcht.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3pivxllnp.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3yrhhtdls.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ldqgfjlj.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3zihpuucm.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3fobsdoqe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3wjhuycni.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oqmxkzkn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zylrlyfv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhnzxrww.html


<!-- 参考信息 -->