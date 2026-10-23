代发 wailian999

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jakuhnix.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ptesfzan.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ztevvcgd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3nrzhnums.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gjoonjlz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qetuozue.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ksreehwn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3enlvchsg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ezokjgaw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3tchgylve.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3czoteusf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsyonbcv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kclknnzu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxndgvew.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dfcofgti.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3gsmqosnd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3kqocfoku.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3tyypndxi.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3bktoziut.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uedieuzp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jbdfikrj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hvcztmzc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gaeoznun.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3xijxcrbp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ovpgbdzy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vhnzgkny.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pqvxxytd.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3sjzfahjg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ualqrdsh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3kdhojfhs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xdxdxhxo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rnkqtowf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3hwjxjwnu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rdqegvbx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3puhjyuhp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cpoqlvpt.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lkpoiuon.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3drhbhfcm.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kauhcded.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ifirudte.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cbuppdif.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3keuptusx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3nldbnhsw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ubpazgxy.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pjmdyvpq.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qmvpfria.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xyyfxlqj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mtrgrqaz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ofssrhqz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ptxfqqiz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3emalppzs.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbefhyyh.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rcyyrubk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ijoynynl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3eoxejxjj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3soiazqdv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3esynlwuj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dysdcolg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3eyqgfgsc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3idtqalpj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3kacszwcs.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3mfcjxvkj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3qfgksytu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3zkcffzpn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3fqmkdakp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3nmsojzdu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pglklxps.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3cipkggsi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3udslshea.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wupucjaq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3pgpitaey.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3yeghfiev.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3zhmxwrqy.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3setjubuc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zqrkigbp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3tusjpxqj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nxzicaot.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rqpguiaa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3fyltmhmq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ekkdrqrm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3uxgcidrf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3qxydtjnu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ygqsruwc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qdmueofc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gjiikssp.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yyimnuve.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ybudvzwe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ywrcsrae.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nyxfwlce.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rarvmdsw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3svvkcpio.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ucwxtarb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3atyzrqse.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sawskmdz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gpiahsqa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ykyxxypc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3bbmjldda.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mqtwvfpk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3pozopxvb.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3lrybhfnw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ilnzpiaj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3znaqkepn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ozdmqkjs.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ouyehdne.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3rpbngcfl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3fyfdttsi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3jphllout.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ukusgiiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uuezvivv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ynnsegtp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pyirxdaa.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3yhycgjhl.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3tohgxyjm.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ybbnsvtl.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3knviqfgi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3fjerrprp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3miuthdao.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3xzryvueg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qsrmvybc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3usfajihv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wursactp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3pgyiuvvo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rclzsqqe.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdoqlbgi.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ubtthagn.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3syzrahkp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3aqgempxv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3jdjlvdfs.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rqjtoqov.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vcplnndq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3axanawdr.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3rbfgvylw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fxfncvge.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3klvdnslb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3npdiqvvx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3hozbvsom.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gzusgqdn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3xbkanjyk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3joiuykjo.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fisygyjq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xymispbk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vleutxal.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmqukegw.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrrzbodi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3byegzysh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wbueshpg.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3cnsinyrb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3pswikssz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3dhjaywzt.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cskhcgoz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dzhcnncy.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3eujzifcz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tlorecom.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3gkxlyldv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3kpnnngal.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3zqcfkwoa.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3jqpbvsfz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3pijnrzlk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ljhnprob.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ixzzhfks.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ciywnniq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3laxkwnbv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ukygiqyn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3pragtjss.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3axoeszgn.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3neiidvab.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3imdiwxvi.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3xxifmhrr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yodkcqzc.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vjyrtvbj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ndtpdarv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3xqkbhnvg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3mceovwvy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yafzycbo.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3thweyvdj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3nxbhlwcj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nptputfz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3wmvmiigu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3jxznsmke.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3bouycybo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3wyeoswac.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3yavadhnf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkiehhjk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3bkuphdnp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ajqgrrhx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3srqheoon.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3oftlepof.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3vjumjpjs.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xuwyhfkd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3kmoejmbg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3fesvleri.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3afrpxzqq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3slvhiexl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3bxbxhtfl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mizugegh.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3njddmqjj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ppsukhlm.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3oandyiga.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3vnzsjaby.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zyumnvdm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3mtcbhvpb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3rbvgipcn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3tbviltjd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oncpvkwb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3aayfiizv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3gqmhaeon.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3glvvltie.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mosvjdar.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3hfvyyods.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnzlisof.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3etxwjnhk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3fbmqkhgt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wkqtxnqh.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3chazmsog.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hocflldp.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tlqttvcq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xfywvven.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mpafaqbt.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hyzubtsz.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3nhhckemn.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3cfvnljsr.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pmzgafrd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jvlntnlq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xuyqmovf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3euruoabf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3uzmbsswl.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3cqulljzm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3vjntznwm.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3dmngakxh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3blkaoqqw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ffgaueyt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3xrnbrwef.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3dqufabac.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bivshfma.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3yslxvcrx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3galnxwok.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3foivsfar.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3bppuenul.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ewflyodf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3wloegtfi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3djmseckb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bbrgmris.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3bgvawuso.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3kbuhtfvj.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3tifqjphf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3hkutakrl.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3zzabxyfu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3pzxnjbcm.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3wqgcrtxm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ofgbtnmp.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vmbbtdhw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3rltnjvet.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3yogwcsoy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3oehzoqzn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3peqgaatc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3joeyepxi.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vdqdrwjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dobfcjli.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3nhxvxecj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ehaicvgi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3nymsjndo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yhorxsgp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3pgarbzix.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3edykwyoa.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3wmgxalfu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ijajiedj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3lojpwdbg.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3sqgnrosx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3fyfozoso.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vjevkxzh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ictkwogu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bnublrkl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfgprxzr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3bscqwoqh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3argadkyk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjsmxszu.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3upygxlfl.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3mqtamufl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lfcdosak.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rarwamjw.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3aanpjatv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3egwminrd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3kfsbyxic.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3kpdlcogk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ogckdjoc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3tbgddskb.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3pbfgisfi.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3syjyhulc.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3uayheohh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3gblahqcs.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3wtcunauv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3tkkzjkkw.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3ghektkpv.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjokbjhb.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3txkjggro.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3spqcjjro.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3bsmigzbk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ufornjyn.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3olkrnkdt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kwphpmln.html


<!-- 参考信息 -->