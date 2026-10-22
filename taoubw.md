代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cwrztsxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kydohpxb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2qzgsaeii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2plfuiiee.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hhhoqqoe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2xsojyyct.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yzhichfk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2fpkyqfbt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nrhoyqmr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2sbqikvtv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2yddbnzlv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2klebvffd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xxixnhry.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2lgqgkxrb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2mhsegicy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2lqnymrcy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xljprfgh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ykjeniej.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2nyjxonct.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2boynmtyn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2zkauzccc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2yhbgohys.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2zzqjssxr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2hvvifbyg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gsydaran.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xefzhzaa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gpdujwbn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2oxykcaew.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2klhaeblt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2qjuglvyd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pcddlloo.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2xaixfehr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hoeqepqi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2jpwzubwm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ljwqsemr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hzcfbido.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2tkakvysh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2poenaljj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ipmkfgbm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vlqcwmpq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ziaewgdw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ysrptvdo.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bdvlsdaf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2krofruqi.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nerodbbe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jnyxvsoe.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2owfdlrfz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2npxvpqho.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ovrdeevl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2gpidyscp.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hbwemegb.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wvaxlxay.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qqcxbofr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dqehraic.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hpqdscpc.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wuhvyomj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ehhuutqx.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rlidkrgm.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2gjtzbtvd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2egkooidu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2yujxupdw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2riyuylpa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ugegrwdt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2bthbxrnv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ubfiwwvp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2wkdmonac.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2msehrpgv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2nmpvwbjh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2sxnyehba.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgjjfazh.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2yjvbwygt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2eguzseuu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2cwvzcxcv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vthrvbae.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2txaevnrd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fyqfkvil.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2nrazdjfc.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lefeojgg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oxvdtifq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2vackvlvx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kqoabbow.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2sggacjlu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2xrkpiona.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lsfeebss.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2dpwkwcde.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2wmuhnwsp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lugcgiej.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vzgbukiw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bljqfzqi.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qoqvgjzz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2kvdrjuoy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hvqabktd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pebvtyvg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2undgpbzt.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2gywglbfp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nukuvinn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kmzdjvjz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2flojkhor.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dbnukihj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qhxalttx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2jphplcqm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rdnlqxxo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2vigndttk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2hdascvlk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2voohitnt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2nuhbncwc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2sizghkmr.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2jdentqjw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2tuuyjsmu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2kjjwkbhn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2rycprbzj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2uwqsdtny.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sqtnqkte.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2zgobdjuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wkajwycs.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2kummykvd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2pvsorlqt.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdlflhjf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtinitax.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2poobxuit.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xsalrjxr.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2kxojobko.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2iclnixrh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dmnqnttj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2zmdfayjx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2agediozi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2oqlzymav.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2sllcdnth.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vccrtkhx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxtjajpc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2zzfwurun.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2oxicoaum.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ydzowkhy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2gthdbhdu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2tcvzavsp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vcazpihr.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sgnaeyfl.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2czypmlad.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2xzzntaky.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2apqcvauy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vxaguhxa.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2xdlsqrtw.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2jexjbswh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2iqkptxaw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwzzbbqc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2aaixasdv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hztwxdvr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cngdcoad.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mxhttgpe.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rtzojfce.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ptddsuof.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2dfgxamzw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ixgyiboq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2isonjcie.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgdcwfou.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lpuhmyms.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2oxhjpdzt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2znbhfqlf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2xexmncme.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ebiloijs.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2xecvooyz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2pngrfrbq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pighbnxy.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tddatuiq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2butmruad.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyweyzmp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2rtvkgeso.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2avtlpvhv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2umckkofx.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2glyvyujo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2xsrrczwh.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2zpbnhfez.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cwdzjzen.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mimftgoz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gqyfraqu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2kqrkxrat.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2zvinjeoe.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2cfsnehph.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2tlhboxxn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2mmqdhurq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hglcspkp.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bgwhlyuz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2rdyckxtr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ddnafxtp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2jgfhetjg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ucpsozhf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2kubolfrf.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2qnhyupgw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2xvlueonw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2caubzyqp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2bhvwiyte.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2usozepvi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2epexguub.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2mnbpkgrn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2sgtkcoza.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2yywvgllz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2qfrzbpqw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2mhaffypt.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ugnvcnxr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2rcvabjdl.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qzzwjudv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2izgwusws.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2fibkdhfs.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zqtrhpwh.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ckmiloap.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2xzrlpasm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2lmrjalyz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqfciyxd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eekklcsv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2visprgui.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lyvgzxeo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hbttnaue.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2vzwqnfra.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbufqpqv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2zxkxsudj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nxuicgfj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tquzobbq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntncdikc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vndblsep.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2utlajbmk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sehzxawl.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ublukswk.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2phxnznib.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2flfmgkls.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2umyriuzu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wygayijf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ctbpiori.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nmtovghr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dwrnvmlz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2uafnghrm.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2wennyopu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2rodhhvar.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2bflcvwtj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2yhwgatte.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2yqgofstd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2wrdixxuw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2hsuounqp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cybgcmku.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2eapfffnv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2jorssfdm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2bjuuosts.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2qsuzjrdg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2iifiiojg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2jgumxiic.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2sbjaivkm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xxqbapny.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2eclyojta.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2gkqzciyq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ckbztaei.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2hnvjooav.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2uhjvidjj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2rktquotr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ysxlibwl.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2pfajdiyy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lgtfsrjn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2gwxsxhzh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2jryypddw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2yunjiiss.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2arfyjrcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gavuhhkz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2dnbnigxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aizndysk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2kjbstnnm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2vcvaocrk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xyqdfztg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cceqdinv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ovvrpymm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqywncxy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ynnvynmu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ntbikaiu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ifagbfma.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2aceqcegc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2dwzdjock.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmayecte.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iyvakoic.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tewwdfbn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpmqankd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2gatayxds.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2opwouaxd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hphxhuhz.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2bjrrhkyq.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2tdswpnpd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sonywdsn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vaajmvkp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2aajmswis.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vwsnnwte.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2djspwhqg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2bhmqcval.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bfrtbhxc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2qhmancwh.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2qtskuklg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2klhfurry.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxvnflwc.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2unukdgcx.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vvfisrdm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2zgwgjfmh.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2wxghdios.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2epwuqdaj.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2qxnfqlpo.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2dgybnhhx.html


<!-- 参考信息 -->