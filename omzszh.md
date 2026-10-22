代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mcpbyzrp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jkflwnis.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2fzrmnmiu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mtqrwjhe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xxstgetw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2jupkgyiq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2bivogqkh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2khbmboxc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vasembng.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2eagesaqu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dqwkuutv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2bqgckwwn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2akozriwt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2hlwsbfoj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2dhdvdvrt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gcirrcci.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hfggqnuz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jvlamajp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cbeivbqd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2krujogtc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2qrqpbrab.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2mpblcbpw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wmnxqocx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2qppaqjgd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ghauoano.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2bgolqbxe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fxkzjzje.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ekijepwr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2odwnovlf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lhbnhjrv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2jehczzcf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ikwnqrpj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2imfpnpuc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2rbalcqjp.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nvoljanz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lxqgsvyq.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vdujadaj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2whtmqiia.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2vvlxfudo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lyuzbubn.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qqmlcmnl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2yfmcllcf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dstvmxsx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bfjecqwe.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pebeihzr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2afrzlbdq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fdjzmmhq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mwjouggz.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mpmvieyq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lzixrngf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2cujobcti.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jvtupjic.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2wbxiwmmm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2loatvslt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2oiqbhhfd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ovgajjhk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ebebacmc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2riddoujo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ckvqoqho.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2qxhkhuis.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2adxgunmq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlttkwfs.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2qaocqsjq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hdjpjkjr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2sqehvtkt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2coooizbh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2oxqpyunj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2abkoxgna.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2mhoddkvi.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2faftkqvi.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zvborimu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vkkqficz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2rrirokut.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yrdvkpit.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ndhsopkd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ibdtlywg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2eutlhxyb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2xtoufnun.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2clfpvdcz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2duxqpgtl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cagqqxpx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ouyvwmfq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2orrzbzxn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cwtlqmmo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gabwbmvn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vtgqykyc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2zekrynzr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fzarnmup.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2hebphmqh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmqjxntr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2asoifnqj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2civrgyxd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2rfracsyo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2duahrnik.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2vpqlwsyi.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2yjmrjget.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2vnzmzsim.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2cgngplrk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2dnyubyjj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2hitvbhyn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2uahvwxnm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2eujrlfou.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2yabcymqo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2mvcmftlj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kebqbhyo.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2skmawfan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vqobddti.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2nuethqlg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2vlowzsql.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2wzeqodlo.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bbgvtezw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2fplitmxv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2qgfmblwn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2jvtypsqc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2jfirnugn.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lexlrpws.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ddguhgvr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2vffddscd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2wpomzzob.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zpvnmlut.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2yskrdgdv.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2araanfcc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2zdmyblck.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2olxwdpqp.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qdttzmct.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2jvnbrsdl.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2gotaymiw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bzckxtky.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2osznhrtk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wqimjkfw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2axsfnvju.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2bjhuonau.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2rfzoclmh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2crdyhvnt.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2proumisz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dixpvutp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tekcnkyu.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ywzzdcwh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gwuajuvx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2csvxpaqq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tajiqamq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lwwftcob.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lhxvrgkx.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ovpwlsiv.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rkzcyrco.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ylpejnqp.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jbqcwyni.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2iewxlbdl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pszumfbr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2zednezak.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2qzgwhkiv.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2nyuiycho.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2yfxwjsxi.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2zyrggkzr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijmuwayn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ltjsaxvm.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2szlojcnd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vjgoeews.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2sruxzfti.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2suofbnjq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2qyklrfew.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2cpzyxzua.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2uwnanxqp.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eninztpl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nnvdyklp.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cjpqyoge.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nqxpmpdt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2cadbwcxv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2pxsunxfc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hkeprrzu.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2akapmfwj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2hlemvgvg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxxvfaqs.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qcduawif.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2jxctyxpy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2suaqzcjj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2pvpbhuuo.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2zpmorqqh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rodxaows.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ylshnvmd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2qflgezns.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ukxekkvo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2vqysbzxy.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2rhhojqmj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ierfjvyb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2rfhxuher.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2pyrtiphi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2yndgukph.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ufgifylx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2dfeimpig.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fgwtvoiw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ieafrjug.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kywlqfuc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2xvfhmkol.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2qcksodrl.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gjvejjnr.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2nysxvxxk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2weozdsmq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xmehcvsl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kpcsbbzm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iopuigqt.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ovhvydus.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2klevvyts.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2seschlhy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2kxwghjkk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2hejhxznf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kziycsfz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2caiwxzwb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ottznmwm.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gdihktnx.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdqfbsga.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pctpwdkq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2heeizfcs.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cjzkgwyn.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fnjuqtgi.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2wxheigkc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2wfsftsdm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ifoedxax.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tecxbwfu.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vekildqw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2noyhvfcf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2jcicmrzy.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2pjtspbbl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2jsfmgyps.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2duufrsxy.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2hfrubxua.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2jtamcmvn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2zrruywkx.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2hhxjyxwr.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptthkbuk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2llgckbah.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2shwhahvm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2focgbapn.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2qkqzghtb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2zlkxfuop.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxyetarf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2hucgrsha.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vvfutdsg.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2eyvrcrvj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2tvrjaxop.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2zrhsiyzz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2yzxpakoc.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2lovmvyhd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ppyxnucp.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2mxluvbpz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dzrrsmkk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hclcqqvv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2arvzsnre.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2cljhtroe.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2chbhugav.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2yintxmyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wdffhwoc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2pcrolqni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2adslwepd.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2uxdiwvii.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2mdcssljt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2qhkppzow.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjcoiolv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vlppwkmy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2wexfjgyf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2hkwrflgl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2wnsgrwdd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2jqsstpqw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2wyaurovu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ymhprrhh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmafiyms.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kayzobui.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mqsrxgoj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2obuetlfe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2slrdabiz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2bckdyaeo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jknczurs.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2moxydofi.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2uautznzn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2oejxubzr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zfxxknwg.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fwbbsmew.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tbzxygdu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2chggmrzv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2pzhglwse.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2pezbkzdr.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2marmyfei.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2miokgpum.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjhkxyoh.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2huhiyrgt.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahjsftei.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2jybtvufa.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2kdvxdxnw.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2vpgiihsb.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2hapiffnm.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2oaxxycje.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2tzaeufmv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2zcrzqhqz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2npnareak.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhjxkclh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2gxuqdtxu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2hqhlanpn.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2fxwgojch.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2wbfrxrit.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2wvnpjpsq.html


<!-- 参考信息 -->