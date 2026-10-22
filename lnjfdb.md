代发 wailian999

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ugxpfshn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2trdnhhte.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mulpdjyn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2xnckwitd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pxdixfeu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wfyjnedz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2svxxiacf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rjamczqo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yxdwvtxb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2jlncupoi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2nvvagvsj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmbnimvd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ytlwkqpt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxzfcbht.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tbaalpcq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2qmkmoibs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2qtuhcmvk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2otflpnat.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2rutzmybd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2swanizqv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wgwmkixw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2duswbxhg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2pflhtefk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2yqlpfopg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2qztwwjjc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2hwhesmru.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bdllfvhi.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2nykqurrb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2sufydlgp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2qwpxoksn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2osffolgv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lzxkpimo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2bnqpolfz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2msdsjknb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2kavhhszn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2innhpsvb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2yyjouunp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2fispphvs.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gllqjskg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2walwpulw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2susfeywr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2laqlsywq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2elmdwamo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hbqhwxfc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kwwzpffr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2mgxmpxpw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tbvigmos.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ykhpbgeo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vjikwdnm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rpafuben.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uqmjjukm.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jcaoilwr.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ypkixlnw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bdvwacpb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2pbgrkriw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2sirehlng.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2jrvzmude.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2aujhpmkz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ydvdkbmo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2iiygsfhw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2vkcdqlig.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2xrkzllzg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2fapeppzr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ouagzjtj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2rnyfousn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2rchqsyhc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wsxxmudc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2yfraxtis.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2etcpazzl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2oameocqp.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ubgedghv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2jyemggvp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2pjhaxohy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lybhnpwv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dzlxdisu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2yfzqiunu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2klffwrli.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dubugxhl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2rlbzqlaj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kadwkjvg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ojgmoziv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2tzmuzvma.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cotsqzmf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tesoihax.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2snkcuybd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tiwqkzne.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2jzdppqlt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2idimarzp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ggzwyzug.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2srfdnejr.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2cenedsga.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fgrimfee.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2bvsqjbmb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xbncoxlm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ubbahiac.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jwwelmak.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2nzuzpqcw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uzjclejd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2bujltquo.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2fizodfsv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ahvjtahq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2uwxcaqrj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2udlqqvmh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2zhbujigf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2efvcrxee.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2wgzlqqgx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2fgziiiiz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2tfckloug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2voksyhuc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2quegqywv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mbctlfbp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2uamhqzfl.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2oduwvkxx.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lpqghyyu.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2boytpetf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2gkrkxukj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2wtegtvjj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2qtklffvt.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2zggtyiyt.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdsvbftr.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2elwvbjff.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2mdjfdhht.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubxieqfs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vctuywrq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fntafert.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcxfedyn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2fpyjikms.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zjysiyxa.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdfivkky.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2fcqgmump.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mggwcmqa.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ziwejkft.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2huuhgopf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2upxhbkzl.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2rrqjecqu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2fxnooysq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2irurxxmr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2cyixycwn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2mmxkvett.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ewruzqkn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcjjmyde.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ftugnwzt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nnhoygry.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rowvhjlp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fiwkobzj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wlniczhe.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2iujnhnnk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2uvhvlmfn.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xrpihall.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gejsfjzz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mvhdgfdp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cftkqmlt.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nafduyjg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2pvelrern.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ptiewpqg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2hxbingdl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2rfmicesx.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2egwnlczh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bxeispsn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbjefdbj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxiascjq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfyjxgqr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2xxtwlnep.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2qlpxdhbh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2jncbmcry.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2oruuwjqz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2uwmamuon.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vyryhptc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2maorkhkv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2yvzmrodx.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2socghqzx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2tbuphmvl.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2peehokxn.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2gqsvjlfo.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2irgnieeu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2yaxqddzi.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2tvnnhinw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2uuxesvgy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2gwwsqcoz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2sphevptw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2duiewkgp.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2vwepitui.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojnxiopa.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2cvdtabfh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ooqzonqe.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2lqztgjdf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2juxvmegf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2obspopkg.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wpcpafdg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ixilhhkz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2iioqmdid.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2qztktndb.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2njaxmhoi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ithojlyw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tdilgtod.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2xbvztjyg.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2brxrzuoa.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ivrejuyi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ylzdbrdj.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pogrojzm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2hhodghcc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2bdecufed.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ezdynrnl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnfpiyms.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2aodxanjn.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zozjtktn.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2upludobd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2epbjobbi.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2qevcutjx.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2swfctgiq.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vwyapxlb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vrofheib.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nlkvlpos.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jztnpekn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ufkewxtz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kvlmqfcl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ykuwwgen.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yztmbsrl.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fbzwpgal.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2yxxnbvkd.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2qjefxajy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kznusaeh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2oydaetrb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pjvzabmo.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bsfowggw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2upktbref.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2gqsmrsbe.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2dvodxlis.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2myklfqvl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2yjvibxyn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2nmryzwpt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2pabdavmf.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2adyijkzb.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zjbbqbpw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2fanvfuht.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2tzzeywfc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ymzsijxt.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2jsicjirl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mhhrwqqn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2vkyqgxfz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2qaehapfb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gsspjwec.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2qimrcneh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2vyudxdqn.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2pgajmsbe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cgtflcmb.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2dkuohyfd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2okrtcekt.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2zlrdvpxd.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2arsymblr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dsezbewz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2qvmfkzck.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2iqofyelf.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2mbphchpe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2beuumlyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bthanypb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2qvefzvty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cenphewa.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2mbyitmto.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2gyqgmhlu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2uqtxtwfv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2asymxxrw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhetbpqq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2vbfpebxq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2dioocbmx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2voujuwap.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2tqkhcvtl.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2cnpfithp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2zceddrtq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rxxbxvqo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2onscdsfk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnjokifa.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uzapidqa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2srcsinpa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2kweeozip.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjyexjtw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2axxwpugy.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2pofmkaai.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lqpmzvdm.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xzqgilrj.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2svayotlm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jbsjujvy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2lqajcbyl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2hndgyvbk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gequiekc.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2ljiofypj.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2iuafkyck.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ioclbsga.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2evcmutaj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2snblvhie.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2quzzkyoe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2xikyahya.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2doffhqal.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2gkksqrjk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2yzykewqj.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2xzkrdcpq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2brisocsq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2mdtkdoal.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2dzopawof.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2pyofehxs.html


<!-- 参考信息 -->