代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2lrjluvfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oftthsqq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2qzdjmtas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eovaclyf.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ewlzqtyp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2puzhdzoi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2doqxsuzh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2cgdabvre.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zepbvowe.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zzlcsmxs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2aoiwywee.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ghdjhzie.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nvqmbpjf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2aqcjfuhf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2nqtsvfya.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2wujivrxz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xiteqgwy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fdwilfpf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2btqrfvqj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2vtanyebv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2sdzmcmha.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2xcbjzisu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2cnyrmtec.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ndhyfndy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2efjltysp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vztobwmk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rjsdcohk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2hijbkdqf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2cdiolvgv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2clyrqpch.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2sigijlcs.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2lkunyjwu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2btplvybr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ceaaxxho.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jqdicbot.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tswcgfel.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ctlpsamb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vgqxfypf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ektwtial.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2nsthpalk.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dptpoelk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2cxgwrbsw.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2avbesxwx.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xxmggxlo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2adcnccnf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rxljvoab.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2lqgeuofs.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lfxyyvrt.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tllidhaj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2yeuaopjl.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xzuaiovp.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wsodyoyz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sbtbytea.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xhagjcxi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wfoiqshh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tyqrcicv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2duuwgnoc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qojzktsa.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ldqpdiwn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cjvxjuvg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2maulzwhd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zqxtyhbp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2acgmxhse.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2dpdoeguk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2wlkltdxx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2knzibqkq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2bxlxujcl.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2mczxqowx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2asscycgw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2qlxmybdh.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xunptoiy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gasalyfq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ocoobvsk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mqhikkvy.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2uixbgpeg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cewbkkbt.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2qaoxvvnn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ococbxkj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2juxumoex.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2liuitsws.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lzwodoxx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ggkxiwwr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2fugishdj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jcowouwg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2mliilwmq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2lnpcvxha.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bokivaol.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hlbqxzsq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rfdftuim.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rtukhmsn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2buczkfbh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2frplzpsj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xexmmoow.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2atymrpey.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2gvhuiurz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2socdfahm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mexzwpvl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2thytthgi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xyvcaqva.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rrtqdvjx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2tbqrfmuk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xaztbtdb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ghabibgs.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2askntqxz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2qrmflphc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2yiuaffyg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2kfdgchqw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2cyaffmgk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2bcqsnyoc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2tozbphvk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2xnmjfhvt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2hnkcpspg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2noeqvlzp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2pixpipad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwagdeqg.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2hrmrosve.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2flirjyxm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfnigefs.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dmowdfvl.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ebtumnha.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbchvffu.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2jdjywfiy.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ukugiwxs.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qhpugcla.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ukuczgtq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2dpbbyjhi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mzetvtsr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkdqgnkn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2cedqnukw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rxlzwzgo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2vdjuajsd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ffjjjhpy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2iiesidto.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2jzpubbpg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vxmqxjxv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wessfpbq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2iaiuhvwd.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dgpscbhq.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2qezmxcmh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2zertcfgf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2gcilifnh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tjkhnuto.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2lfqtehdk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2tpuvvaiq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hsscaxki.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ipxbmrzc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2aoirepfo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vqljcnkt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uswjrzxc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2eqkbrryk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2cawoohfu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2dhuxvwac.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2fbnnehru.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzzfhsoz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tcocjhli.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2miykruyo.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hfnwftda.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2mlypqcir.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qycmhmea.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2zsojeqfv.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2dzpnxsjk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2qclrwyxa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdrkosma.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rytyanfb.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2shilaunz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2atviprfz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2cuvldeun.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2zerqzydf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2mbjdgesy.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2gwjthzqf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2kzodyrei.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2thwqsgiq.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bwujtqxk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2asdmxiep.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gftomdgl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2zfekonfx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2txhqcsoc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wrsekcda.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2ksukgncv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2soqsptfk.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2fbcalolq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qzyhyvvj.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2bwykbvfa.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ivyqrjke.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2txrxzjmf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2fcjbvugh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2joylacsw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2uvutvrlw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2cjyrqods.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2csyotban.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2msjojhyw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2zydmlrcc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwjqdlqs.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ohyheuts.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2wirysano.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2iemdbiie.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2zpfruchk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2rfossdla.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2oqceggli.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2obedxyxx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2biyjpgfg.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ifknrgyh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ckaonfyc.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vvpkrlnu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2xlehckze.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2asywvzld.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2pqmghait.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iolpyfiv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2edxsqksf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyzglgjy.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcgqpmka.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2llnnhqun.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2panmeshb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqvdbqdc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ewowxibv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2oqlwyiyw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgxpjnsp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbhdqhdk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yoppkgme.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sudbxqsx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vsabvnbx.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yzlnimuh.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tyaplcpl.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ltcxooha.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2zeljqaqj.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vkshkfft.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bqkrkvak.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pmtuhmtm.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jzjyjspg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2yqwmvtga.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2dfwofpps.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2pgdamslx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2wsbwlkey.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2virodkpe.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2bcgybznw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2iopbeofw.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2hzdtwxrn.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2duriblso.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2zuhpruqy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2vhimnzgf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2cqodzbyq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yaaegsnm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2bvieutpb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2crwmxbua.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2jydxipfq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2drliacwa.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2lbpimvqp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2leabnnla.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2awxivweg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2seynrdye.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2bphinlgx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2zlcxglbo.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2kbcmiiqp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2vorsbosy.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kiqbzhqm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2khnhgevy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2okgusgbt.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2yxibdgra.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2yvxlxmwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ywnbdbgw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2mdxszywe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yuijrbwe.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ujkdwmvp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2qukjljtv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2wuumynxo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xkbwupqq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2hlcsdaww.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2nmpqbxub.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2lfrzmxsp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2vyttkniu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2wikrpyhz.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2yqeoksqc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2tfpxxiaa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2uazfnruf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2crnonbuc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hobkdzib.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhwtllxh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2gyjyfcik.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2uexonlvq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tazuxkub.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2cnvrzyhw.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2vslvznlm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sooccjfl.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nuzkdctb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sniuyjqs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mktzmkas.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2juxdhrnt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2jdyzjhmo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qtqwcvaz.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2idhirzyo.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2foudwddq.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wdhcauqv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2rwkcewxn.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjfgsddj.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2rhyveeul.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ivabxjnc.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2eskbhznh.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2hjyvecsy.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2vuffgmjz.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2zfjkyuaj.html


<!-- 参考信息 -->