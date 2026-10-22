代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uzhermik.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gunsuugi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2kstnleks.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pacrgbvd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2mtdyrwhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2loskcjej.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2edssjpxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sxtwofyi.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ydiilzjx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2thcbwmfv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mpxixnhj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2axsfqsma.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lmntioqh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gfjayroa.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2fpfqowcp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tybytomf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zafolsfl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2htrciikv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2bfyglaog.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2fwaqhaly.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2lyjzriiy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2voaxwsgr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2iatgevrw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2uygsznkc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2pplqpzlf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2yaswrnmz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2dsiuzzcf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2eoxjxrdi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vpqlmxep.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yakqajcw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lodtlmiz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2myaevdlv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ejbsekhd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2dvualntk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ckihggou.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2atkfxmgt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tdkhpkzx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2luxwfcfw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qiubqgdd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xxpfxwsr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2udqrgtqm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oycfrplj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2dogbubza.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2sdqmpjgj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2jxqopzsy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2yzthvefg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2plhdhaaq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jhufxdrq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mrwocqkr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2eizmqwlv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2phvellou.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zmubsrdv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ieoyfqrh.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ofabunsw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wrfkxigl.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zmwprtbz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2faplxfvj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ynhmgbzd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wjoluoeq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yizrkbje.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2buncxyhu.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2csijirng.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2podtfgtw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lwxabafm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lcgelcrt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2yrvksior.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2gxqhprip.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2oegteilk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2nqekepdq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2wuvsfbid.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2kotnbqbi.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2iebmuvbe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2aixkokur.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2zcqbpsbb.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2axtkbslz.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gylvhmjq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2savsyrsi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2niqdccpa.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2upvcoibh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2aqyzjvfy.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2lmooyian.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kmqbfbgo.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eyelbcpt.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ckrswwrd.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hxttbjzw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2efhlfssq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2cpostqdc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ziqpdudh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2xojfweqw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2bibxvotm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tfonaqmb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ryrlxoej.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hxzzkhcx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uldccqgp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2wjdadtqv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wcfxwwrr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vqbibmlo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bdufrkaj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2djnxkzyl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qnvcxxpl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2hzeuluny.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2euwnhrwn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ukqjayey.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dmohuryo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2eowypihl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mhmmnzit.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2yathcsyh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ybidcjpl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ctkhpahk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2haakrwgz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2cqnmbcya.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2akorydtj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2cwixlnmn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2yadxzosf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2etgldvam.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2uydbygrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kthrnvua.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2vdothhmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uqvpyiff.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2xzaerltk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2xsrwkjhe.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jboajolk.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2npiffrrw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqpeytjn.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2dvitzrtq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2sqmrawpf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bcupncus.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2tbrqihiq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ipcbyrro.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2cskguvmu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2zykcfhhn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gdegajuh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2pmpzmobf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqqmhtur.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2qitddhal.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2keouwirf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzdsycri.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2quuylhzg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2innidqow.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wvkrdqml.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xcygaflr.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2spiemgvr.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2vshdffmf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2yvviyrwz.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fpvvnlbu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2qredwrvj.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ctwqynzz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ijwyinyx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkohdjub.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xwmagngx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gmrhcbgh.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yczfkfax.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kdnuepla.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ttiobkmp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qefrfhjv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2aazxogih.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2udzombqn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2btcukiyz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xgocpoqb.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dlqxspdg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jkcsymei.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2twfnlhms.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2gzayswgj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2bhbmkdqf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ftnswfhy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2mxnjqmwv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gqttzenl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gssespqx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vnelaxry.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcnypvqm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2tzcujcla.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2midtvejz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2aagwqqev.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2yagtawzw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ifrvvsbl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2fznenbcc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2oykhejzb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jnqelvxp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pihjroko.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2znjzgeon.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2mdnccitc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oxiptccj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2bzwlzvvv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2kmpyykbw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2krmpqume.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2idthnshu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2xbfeeedq.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fkaybueg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2uqmsepef.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2xtekdvrn.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2vtfefdnn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2blpwgytz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2oiypytrf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2betjrjfl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2mmsrgaxp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2empsigyn.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2mayzcspt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2yokfmtpn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2lytewntu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2oyjjcwub.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2llhvdcen.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2bmtoaagk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dccfgkiz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ppvkpnei.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tvwhvyoh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2elgxjaos.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2dvqcgrdq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mzblppim.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2hfwqebvf.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ayfxjwpd.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2vhrwypec.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2whnduszk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rztsrazt.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ridfcmfg.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2atcqdtjn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ooiflypa.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2pibbtjpb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2qpjhxtth.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dguwbsfc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ydpiggrl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzoizqkg.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kysnqzsv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2adynpilk.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qckwnpwk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kwmxsgpn.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fjumxeve.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jhaclpcv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2pyfldcfb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2gxpqibrb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2neqpofxh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2urquczpb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2paosxnaf.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2klychkoo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2dnpzggfu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2iooolslv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2czsmazzl.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2rvjbxday.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ekerexlo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2kusphmzu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2lsdcllwz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2fdrawppi.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2uohfwioi.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2xnjgkfby.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2xaicyzle.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2rzjtdijl.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2qucdtjxs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tqaxnncq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ailmpgsw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ezsybhej.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qwtbqmib.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2rjphbopt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2jxszlmcd.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2qjyfinqe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ufvobiae.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2hpjosyrh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ufcuqgff.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2hzwaspzr.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dqzouvhg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wbmyyxxj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2hazbyvkw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2bvcegjbx.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2xyvnidzn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2oqfmigkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hxfybely.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ogjnevud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rknqpnew.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2moptwlgc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2qlubczar.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwjpxnqz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcxqlbhv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2utgnxjzn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2fpigmqqg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2xdbqaiyo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2xcglinqw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2xgwnxrqp.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2bumrhnem.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2loxciqco.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjdfddbb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2roycnzkh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vcnnnpei.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uybvznnz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2faflsviq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ibwqnkko.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2auywlfyy.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2gscgjjkh.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2glgdjgzp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ihlkkhjg.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2lcuxmoan.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jtkbbwbl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ifsampmu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2zetlxyyj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2krkbiprc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2railltpn.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2bzapxtzx.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2bfdeysii.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2oojtpxsj.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2chcaiflm.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqzxotgh.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2fzzeujum.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2zhncipki.html


<!-- 参考信息 -->