代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3tsgkizmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zfozeqbe.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3xhuqsbcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iwzcexop.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3aiqwlbyt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ihsnseiw.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fioknhcw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3eugzlein.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tzgogxxl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uamhzpvc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3axfjqclf.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pmbljcns.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pwyfmyrz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3yqodsyhg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3qwpqofia.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3fbjcxpxa.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3fpxjqfzy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hrhqyabd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3mpajpvup.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3pyxlxwqq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3svohxtoo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbafhaxg.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3mxywbmul.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3gbfuzsop.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fxkzxipo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nouqcywf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pnntggmt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wcfrworf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3twttvdoj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ktajcndg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yzfkypxe.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ycipuajj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3loxpkzsg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3eokdtuur.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vdmxnoki.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jmnqmzvf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3dgydvqox.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3pdgbcstx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ojmuyopn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fsrepqky.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3lemxemlh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3jqchmvua.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3remjrctq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zqnzdmla.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3csgijqdt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xjotqbvi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3hejmeqdf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pbgkwmvc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3noeefszy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ctglctxk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yldytpox.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zgetilhz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3onbdtyzy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qsvjbpli.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zaarlssq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3walnixex.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mnlivfdw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vsamqwlt.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ajmpupdt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fivmljwi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3hwlofage.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nqyafaww.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rogmytvg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3mghsmzma.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3zddsyrmy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3mjihgipc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3uunvbhbp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3lnsbgiyd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3hvfbewdk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3epwtgxax.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3lysmeuoa.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wqhbvvsb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3pnbxxxkq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tmvnbyww.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3kmenfhno.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3lyimgfmm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3wzncnaou.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nmkksilg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3crhkceaa.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3cjkfxvrx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vcildntd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uqydwnnv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3myqdusjg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lqcoyzih.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3kqbwkyut.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3bsepwxqq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ptrofzfo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3udkfvfyv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pymglomn.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hbdnoaeb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3jcxnxtmo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cuolkglt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gvhvxhko.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pbopzyzn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3htrklxfj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mgkvxrvc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ifrlvdwk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hlljmcaa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3doptghuv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cjdehnst.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3etlpqbwx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gphezttx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3vbqsgkim.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3hrhoawfw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3kgmousyk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3decrhxib.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3epvytuib.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ufovmqey.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3tilmcgqp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ixyxelfi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3nvzqztlg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zuytgjmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrwtbyjq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3rfsoteas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3teneakfx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3niulnofa.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3mbjfccwz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3yjebdszb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3tuxfepfd.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwfxafbz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3sqbfrldl.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3iiargvtr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3eqosqyjy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3dgyjhtye.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ldoleclk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3zwnvxyia.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pjdonrpv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rwthmvtv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wvoebvut.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3umwzfcdv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3wxiwbrgq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3rddyohtu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjnxselk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3dglcpbgc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wdgxlgwq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jvrjhlaq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3keddeyzh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gycdrcym.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3oyjvzqzt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3rjbwhwsh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rabdqplp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3vbhlxqis.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ikhrsbca.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pdasijjv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xacjmeau.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlhvbaex.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yjsnikjz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lyiknndj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3btybpukw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3sjeqidth.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3grgomdjd.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3hyszxlrs.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qkltncez.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tjhtgtzs.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ldjdmiuk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hvgycyma.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cvtoicnx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3xwlxzhat.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3yomcxvua.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ghbsuxqy.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3bvdjgbik.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3kpgomjmn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ndhebbsw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jayqusyz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mlioswuc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wioyqvof.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3lqwarbfy.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3qwxeoxay.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3xwddzspj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3nxnnrxgk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ajuwplha.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3acqsesxw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vsgfrbaf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gxwemsgm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3setfubbi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3gyumifsl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3zcdpndmg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qlqtyjyj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3fdwmknes.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3qronxiec.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3aoqqzybx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3jqfcyzxk.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3dmramkuq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3lortjykf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3pmgippar.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3inwfhrff.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ssulhknd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3qxebqqku.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3hjosuxkv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3fanpragd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3wxnovdyl.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3bldvfxmx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ybbhgosj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3pjewxukf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3jzprzgcm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgcwdbra.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3xptyvmmm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3uddwpvst.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3unbaxdlt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3kgcuhohs.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pyyhrwek.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3jfelejay.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ypulphwj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3diwlpvld.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3iywolbzn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3bevfuipg.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3gmkhzcst.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3prbjdthr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3uilngfcx.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fzpgnqag.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bnlsaazp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wdjyjpcf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3sasfmkgf.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3sniwvvdx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fzjjwqkb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mdozhhne.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfysyvil.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sffsmbqf.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bsulapok.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vduzvdzd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dswvssbq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bhjtxijo.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3epcjjmks.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3jabjbzxn.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3mtgcbyav.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rrvukjkp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yeuxqgzw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3huzleksg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lnueeefj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3xkdxtjaq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3clmdkovi.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3stpqwjbr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3rwcdjvky.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3lbersnnm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3tihmnrbb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3kojxqcri.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3lusdrmuk.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3cbukdryj.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3wpjfbjpr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3aszzvuro.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ynvrlzqq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3oziqowsb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3wtfusngt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyueghnf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3bdsdziph.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3miwirtwb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ngedvrdj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3lohaentg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3nnjboccu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3gtmqyroj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3bbfsplrj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3fkznisvn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3tcqrqgja.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jtyqbmua.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ffjnrfui.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3fukpjhyk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3mfhidiaq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3kawmjixx.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3rlaehyox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3buridgxa.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3dbqwxiep.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tebedjos.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3rycxpyba.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hyvdngip.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzjztjhf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wxvvteoa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gwdqmiox.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3tegybnbh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3iepswbcg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3inyzyoxr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3phfmpvxw.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ojscufml.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3xydcgytp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3skokflnb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hhcuwkhg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ctieecnu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ybkgjncn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ndsbmmsn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3hvsqvzrs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3alggzpkq.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3puwgsjps.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3fyygxrpn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uicbylby.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bvrrdwnh.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3zumgukyl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uatlbyeb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3wnamryxx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3clkgrygt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3aeoogkgd.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3rpmrmhwg.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xqbhhbov.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3fnfcyrnm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hruqdbzs.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3migycbae.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3scbksppd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ckubdopf.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3rpcfbyux.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwduhpyd.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3znpvuowc.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3lwkdnjgl.html


<!-- 参考信息 -->