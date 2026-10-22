代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ppyyispq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugumndez.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2eaqesbzi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdflcmog.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2fwmyhkpv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2opoudfod.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wuoonrds.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2jkpnemst.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gsepepwc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lnfvcffe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2canlseww.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nkgknnsv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jygkjjpi.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2jpvpzhud.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2faeeyrzq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2dhrhwojr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hpiijxsa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xunfcifa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vvemhwdn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2djvtttzy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2zvqsgqsk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2cvlrhtyd.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2rpfjiqef.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2wjlgcicg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2tgpqapfp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ledielpr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rvkyzlxo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2aczojnem.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2tjvjmpxh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2vwrmatgk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hdgcnojk.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2pgtonkhk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rdlpwqzp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2menhdoin.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vqnsewpc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kclyutqb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2yehjthpu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2deiiqauk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2szkkrqkc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ybrwamyd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2drmlntsu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2jslzcbqp.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mqbjtqor.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kntpnnoh.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ymxvavlw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fqvmmmuo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2pnooxsrz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cqxcgifs.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zsqpzlbh.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2usfqdjtw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uwfrsdlj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pmoufkap.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qpxrlwdu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2phrcglns.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hbfqdwtp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jftyknaj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2naneqlvp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aiuqjvlf.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2spkdlkhk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jnxqzasx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2niewffkn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2hnedtkcx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2sddoqerk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2yhcwyvli.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2dmnowhry.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2otnwrcdx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2cshjluwi.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2mubnzfaq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2sdfeleqg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2talgwxgu.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xzvjnexr.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2imxkvpji.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xabixwfv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2xhgegjrb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ddrjstty.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2vnnsajcv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2nxddrqxy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2skwwfdux.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dfacmqkx.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nvptrjpa.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fmgtwmla.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2omiezvpu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2lbpznrph.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oveqahwl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2zdjhwsev.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2vwtspprq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jzfjdolz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ehuhnusu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vyydklzt.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dibryxbx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2rosgvlhm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cbdojxqw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ryripeqi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qhlfjrgc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2jnigkgin.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qgtkcsmq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tqqljaxl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wqxuuhwb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cxafiwjp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ioflmrbf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2uihaixct.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2moonhzen.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2brdijsph.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2fvoucqqq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2gxisocoq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2tadcdtot.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2qcqenwju.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2fupbafcf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2pennyklt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2xkzgeibd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2azdqjdvz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2litieenq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aptopqpi.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2zjwibumq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ppmsjamo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2chxglhqu.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2jnpftazo.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2esvwlckj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuqnwcqa.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2qpuuzdjd.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2rkvyjfoj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2vklmmjgd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vyisixur.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tarodvup.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cdtbgmwe.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2whkquqvr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2bineadzc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjlzabth.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldruqpbu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2alyowxkm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2mwcucmqn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2phdknasu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2egjadeqa.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2fnwxsnbu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zekwhkzp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2blcboxhp.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2sspwultd.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tbpvevej.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2chgokvui.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ifegpqpa.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2pokukfdz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2uewbstrp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2nzhpfjzf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ofaepxse.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqratkyc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tqwufriz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lobhqcje.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2apetlnwa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ewwagiwm.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mgspatmi.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ivcxffnj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ruyogliz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2iiqregzz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fouargkq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zkqmdioi.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nayuamxe.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vdxayamp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2rksovatq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vyjmmlrs.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pnqtnvox.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2esimqwtc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2fygkcebg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzzomxxt.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfyjiwlm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zopcbsra.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2urcrbrcq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2pdkpoaib.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2zahshtgx.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ovzocasd.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2rsasraph.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ifedgdeo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2nmjecbtk.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ltycnvyg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wgldcjqg.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mjjvlwgw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2aknjjptf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2fszpapxo.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2pdcceeyi.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ygckqqwu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2cowlbney.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2yglcqfug.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2srbvvedu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2haazkggc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfjwfchb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2frbavcfj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2wvylgbbl.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2eiarzrfp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2sghqiyuc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2rciatpsl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtszcagn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2hoghageb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnfxfduw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztqofena.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2gsovzfod.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2xiixqozi.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wqjacmsr.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2qamaqcbk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2zhnrrcya.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qlpfkdtw.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2dbqgkdiz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hvovchsl.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2sfclpikr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2dtbrjlon.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ephnsvyg.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2rnszbwng.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2myenbdmk.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2mvdieokd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vrrtyhiq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2hcrwwzpu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmzwyqpy.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pqnjasjh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fxsksaav.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2nyubrmpi.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2yadoenfb.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kacxjpfk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lxsovyvi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qssdpeyt.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bfybrilj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fpvedibc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhzknpdy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ieesxmyt.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2upzkmlzn.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2iziubtqr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2wdcqahvg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2pbeknfzt.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2blmothwf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wmimmoxe.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wqtsreem.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dlhrgksp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2fznubiuz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2qjfcxdez.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2wcnzqogx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2iwjwhecc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2xpdhquae.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ccbhjuyh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2tushglgj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2gpxxobme.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2boqgakgn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2nvslvqnb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2nmpaicai.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2bhyaprfq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ugjrsurv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xsjuvfyg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqxjsgye.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2pvsjfrww.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kpisuasy.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2czacxxca.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2tdeaptgc.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2rjnjneab.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mnjemtmz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2mikcisbe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2dzooqunr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2guwkwdwu.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jgkekwrq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zkohdbsn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2uozkzpvk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2hevbbest.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2etylcsml.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2egoiygal.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xmapagye.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2jvnkybmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sqyxrlmk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2sunwzvox.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2icpsctzx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bmpjxgae.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2akchlzmc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hicyogni.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2sqghupso.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2eivmyviz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2chmhhfgc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjurofvf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2hifdfgqh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2rbzumiin.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gkgtnokv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vsamtvbo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fieqszul.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2vyrmbgch.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2vlkpdlfh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2yzmnaxue.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2idgvqfvq.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2nmkylhou.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2vudgobyw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zvvjxbpy.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wkyvxnyc.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2kkuijawu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mockjfya.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2jhqeqpxw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2dsbzsobf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qqpqmkac.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2gxypahzw.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2onidpexs.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjwtbzgt.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xlostekj.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2jxjieyxm.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2xwzfxlxn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2jnkdvtas.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2qbankfhm.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldbkofns.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2deixfmat.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2olnuavwd.html


<!-- 参考信息 -->