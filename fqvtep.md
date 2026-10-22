代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jnddimlr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qhknihff.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2odwwaydk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ppsyciwo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2duywhmsk.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ngaplgka.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2qileshhd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rybthfov.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2lggwdkwr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jphspkgs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2tvtwkdkl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2iblzuryo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2hahskuiq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2etcjzxuz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2uriypfkc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2miasmpld.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qkegrvmq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fzrdwvrl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2miownfow.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hludvgmi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2axrpnpwf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2aljheghf.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tnqmwxbx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2mrytbgpj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jdyftviv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2htmppwun.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zhtffniz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zbvridhj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ypfiaryj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xthlpcmv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2njbabqii.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ruekrzzc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2wrbwgrfz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2qwemsdhj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vtprspbg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uhunvxlq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lmzhxymf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gxctufig.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2jlusnkde.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lnnvshxh.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2veqphfmm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2zeocqjpa.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2znlnomos.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pccuipgy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2izgzrxbp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sqcbpfuf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dpclzhqw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mylxvljr.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zdrkbkbb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2twxgtukm.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2luponwtp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ibtshine.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2cjtlpazo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2nnvngfbp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2sdmgkate.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2iehbevnu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2coywxlkh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2alxumkev.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2hbdcvxvs.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2tdpjqlob.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2whkjjhsj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2yljuljkx.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2htiepumc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2oqffogyd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2klhlpqle.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2bkzqepis.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2eagnvvtt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2teijoadw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2chwmsjan.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xuqzhesi.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2exyjacnm.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2erylfvzy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2naaekjpz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hmmhrpjf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2dqhlryau.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jbmizrgx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2wynsdrsw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2dzyuxlfd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2djxmfevh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uihyrenr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uilaztzs.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jgbutxln.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2nyywclzt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jbegeejg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ouzedrbn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rkxjofrh.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2hzuofwbt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yherbsuv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2owlgugvq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wdprmfow.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rtciapgk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2owbrswjr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2jwlufwqi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kqveaxuo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2fjxoqemn.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2caurzevs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2vmfukyuh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2eldftwlu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2gjnkixfn.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2gcgaxdhv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2jnshpiwq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2pvzfayoy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2mgwbedcd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2jqyaisay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ezafwfyr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ogtpjyjt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xezxefjm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2nffjaafk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2nsfuxdqy.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2itqsviet.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oidzpnuy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2oarofvym.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkhkeskt.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2phtmadqo.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2hwzhrzbk.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2owaifntx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zpktogid.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2jabtfoat.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlcyslut.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlxfrisx.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2caznqvan.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xjbayycd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2otpgdnkr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2jbxuxkqa.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2geuembhs.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2vhhtfhcj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2crxkziam.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rqhnpgbx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fylwssle.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jtdmsfum.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2llrugzll.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2bgundtlc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2poqomnam.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mxmihmhg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2araptquc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2phmyuyha.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uaoylfwb.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2udgoplal.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tiapxghs.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2arulaorr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2shmlyjhl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wyayomen.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ehlnakzy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2qeizdfom.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2omktccgf.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bitypagr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dmdgwiyr.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zthxqqbf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uixrelor.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2vqqydkzr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2wtjqzpgy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aklukott.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2iexewwal.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2zthzyqjn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqfcackk.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2evjlnxsc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rnraobkc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xnuliaum.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2mneqycfv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2dxyhpopf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2xntkznfs.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2negphrla.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ttwciofe.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kfwlprdo.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nzevcrdr.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dnswshwl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eujghbxy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2zhohoxjw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vavffnmn.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2wywikrac.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2kzadojfd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2xmrstvxz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gleladgf.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bepkbseg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2zdgfoeem.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2kkqctwhq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2bfufylpd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2rclgpaky.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2trmhbpob.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2cbthtfon.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2qusqiubo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2yurewqkz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2enzazifj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2zeiajjtp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2kagwyqqn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ttwfxovx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2dgxdxjwe.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xovhiria.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2lekzxpej.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2zwhzxwnb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qqjifnwc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2dfeuuypa.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hakhdwdo.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2smlwnmnv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2zdskewwx.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2frwpmdhm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2nypybasr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2rqqaxkty.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2bbvbbuem.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbyigcxq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kstivkbr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2emekemdq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2avamnktl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2umrmptsz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2jxtfktmi.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2fmolivyk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ozrdypep.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fjitlcsg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufcwboht.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rnrrahll.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2utxkdekn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2urhgssvi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2weonfxhc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rjdiyyab.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mjrkujvd.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2fxyejgkc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2fghmfibc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zvnumdeo.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jumiphon.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2follfsby.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pvmuxxyf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2hpgyojxx.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2hdvswnsi.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2awutfxpv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2iwrzqboi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2zhxaqdqi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2tcgwumfd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2rnxrrlpt.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2hhqxcbct.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2vrrgxadw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ayxepoxc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2yardzzgq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2bjjerctt.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2kpvpyomt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2phrrcokh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2jajueqxq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ytejdhuv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2knufjpze.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2nxpdnrab.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2xftcvewc.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ildotrwk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2upcxdfdg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2qefywgoj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2risgathq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2rsmxmfja.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2bwssvcxo.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ggpjhmje.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2dxsipzlk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2rcwnrgiz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ynkojjpw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gomvcktv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gzlxzmep.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2dqoibosi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahlgippx.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2gqnenvhs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ocphbsic.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sdohubjp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vttsixyd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2rfcwhumq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2jlcqbfwo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2tiuicuoh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2bgggsooh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfrjhbmj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2fczgawud.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2qnxdoajb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlzftpzr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2laaiezgu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nzeqmkea.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jcxjepgt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2nyenoqbt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2icssuwqb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pmtovxzm.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2dvnfwgsi.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2jcdigvfo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2agqvltaf.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rejtnjzb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2oetzfyjx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xdxanmxj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ldflavcr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2plblftdm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2paapaimj.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2vdqrlryh.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jljsyxgu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2tvtuhaya.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2rltvjjmb.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2cbnvgcqv.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2vjaqhjda.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2nyxiiget.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2cgykoloz.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2jsmqulkl.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2lhiborrw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2hrhazcil.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2nvprsvam.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2asukcyrr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhhgbmru.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eujlpsam.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2izkkxxzr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2lsijjkdn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2logdlowb.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ysynusji.html


<!-- 参考信息 -->