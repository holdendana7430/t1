代发 wailian999

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mwhrbzlg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2toxyqdzf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fcfladye.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2cluzkhlg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2pnndqdql.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2asrikwdu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2wtlsjvdp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rtgqpbpb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2knqrovuz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2eracfmre.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2qeyrhwlp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2pskrmhjg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aahczoec.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xrnfwavq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kvondxqz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2wgfslyyk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2hnachkxt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgqtdomd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2wrcpwmfm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2gglmtjce.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2iszucgcw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2leituqkj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mfqebgim.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2vbrkydfc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2snvqpglx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2moyzgsgx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nflfspnt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2blzjqbpk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zskgpcch.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2cmmessjp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mqdnkdxq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bmncuggn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2nmuexkhr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ebmvkull.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2lgozjbqn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ndjbxtft.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2tvssreoq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2aiizktlo.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2audvzhow.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kosvxmfz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2frwkjpwb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wcbtztew.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2aslfwqup.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2arewkqar.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pziyzkrz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2dkscxvnv.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vferfqas.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hdahlycq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tvfnkryw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lmrmfneu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2veshkbvi.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xjuohdsw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zcizcqzt.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2scmpobpl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2jnvbenwd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qanesywo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2khudcaiq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rxlqhizg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2upauukdx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2hbfzghvq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2igsmtits.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2wjgbuabi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2nqwyyrvr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2pfwgndbf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2toetibbt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqdggttv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zuqroehy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2yhiwstmw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ipnnkluo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2lpcnwwgl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2csmapedi.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2zbgohlov.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2hyjbokwu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wfptkvaj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2turfxltm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2irssceig.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lebuitng.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qifwtbey.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2wquujjdb.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hrbxxens.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2nqawqtuq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2dgbwlxzz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xdkgahop.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tzfsogxn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2omgqigeo.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iixpqmkd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2tkzzsbnr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kflmxrkn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sstezrin.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vbgmdiiw.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2beuelres.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qyvzmzqw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2bwpvedtr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dcyvktkw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lmfxmvxq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bwxfemdi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2jejthacx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hikudqzm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ekyrpagq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2lhbcovnz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2yuqymwqs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2uygcerdx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2oargjzyp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2yygqcxyg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2hibwselj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2rrvcywzc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2gqkfgrib.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2jibhcsnb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oqxkogxi.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2oisuzmsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gudiidpm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2dbouzsgb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2gauhcmco.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bvwbutgx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2shdwhcjx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2vfmkjcsa.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bypmtskl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2iyqekhiz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2loemgwnb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekvvggql.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2usefdzhl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ilwyrruc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2xhvexfzq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2oxrrckyt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2uihsupun.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xsdngugs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2meyvampy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2apncyygg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zwrkiimm.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2vbganpjr.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2cswqqwzj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qrovtkhg.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fwbhakxp.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2bymqxlqg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2hihendiy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2qglnuyqy.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2iyjdwwmq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2emeyxtbh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2mseumxef.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zavtzqef.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2owrdnvwi.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfuicjsw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2daclhwcc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcgivfjq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2blyuaicr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zphaiasz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2npqdqjap.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2vlqduccn.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2yfmjkabr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbquduuk.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lznabqzg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lnlhfeba.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2twvrbnwe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2jimfehkx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2frflimpz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2funrfwlu.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2bxejgbok.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2uundyniu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ujfjyske.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wsodoift.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgtvyhxi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lafdkquv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2sjynpdkq.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2pmcifmvs.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2icrwngig.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ersewbel.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2jofwezmg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2watsqwxk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mtqskvai.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kszgssgk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2btbadnes.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2vlcpldjk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2mlygeskh.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2edjsgjqj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2dwaoganp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2houeikov.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2kcceitar.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vupfvipm.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2uegnntpr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2hqmblpkn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2mknxptiz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2lsxtowtd.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2udctdhoq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2dforrzxy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2mltlnmlf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqsjweef.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2sqlcwqyu.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2lcwvgmnm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqslvpdl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2eysmpxxs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2rlkeijwu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xygxmudi.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2mhynvhuf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2jfhqykbg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hfzpxojz.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2zmzdmkxd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2meuwwiqp.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2onbugowi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2jaaaeajt.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xppinfxg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2qhngafar.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2yztgrmyk.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ddoipoqi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tdnvbeuo.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jivaegte.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2hrwcruyz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2keufvccl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zzzlzexu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2xgskdhub.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayrpdncm.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2owwhwumu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wvxmctlc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zkzacvmb.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oevnteih.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wscxbonc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mirfbzra.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kifebebh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yxvilsus.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rbgyqinb.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2kbmhoulz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2dfylypbh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jabotmyc.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mnqambvk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zfxureci.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cafdbnno.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2idclmcxo.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2pszpsrjw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ohlrojij.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2pslsjbyd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2vwssloov.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2krbdaolv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2jhaotgty.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2gpaiqotl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2oeolwdcl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2kvlslbpp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2enncasbl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2oclzgfyb.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qmafqhek.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2kadrskwt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcwnanei.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2zdiaiehf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2njsawybv.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2iqzmducq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2rovwtlas.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ovwjleeh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2nlcaposu.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2rgnjimwt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2kzhihfyl.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2jxyarglk.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jnichkxc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wznukaeg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2twkneayu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2jkivkvpj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2sbnyhiuf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2abkbvghi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ymnjfmfq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2odqbqjhz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pawbdmxf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ymyofjjw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2icyodhsh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2jbserkue.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2cukrhluu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2izqisveo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2kilihmuj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2wkuvfspr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2xaqgotfu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2pqxmbroj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2iicialgc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2emfyvibd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xcacdfpm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2sjfvujgc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hncreydv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pacxqufp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2nzsucvjw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2rpaecbit.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pedfcxjs.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2pxyuekjw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qtcbjpmt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2epygrtfp.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2vapmldtv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2mgujdbrw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ubqbnsuv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2jnoichkn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2dhueakda.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2glukzdzv.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ccluqoym.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2nffihbrp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnxjalew.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2fttqvmyw.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2jejrfcfe.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2kewqserf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2zlixxopq.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2xupewtwm.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2hprzajiu.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2mfaqzbnm.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2tiwnzuot.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ugpstpgb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxoxkbgt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2twlrbpgy.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2wtlufeod.html


<!-- 参考信息 -->