代发 wailian999

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2itofhttq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2xtajoagb.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uinmgqse.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2mesvwthf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2twiecujm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2otrozzwy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2vvgebjxu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2luwolosw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pqspteuu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2esdehnid.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2bnlrfemk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2utluwcos.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2izvxaupw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bauqzriq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jidaavxv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2obfmdltv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2umxrhtaj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2wndqpckg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2dgycslki.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2atpsisqf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vrvkuzfz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2sjndktbp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yjjlzjwl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vvujhxod.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2pqvduenu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2mqvelpkg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2reisefeg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2euvkdaue.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2stkbuxmi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2tuqqlmks.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tjthwewv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kqagtrac.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2lvokqkkh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2casqhinz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2iciczlar.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2kxiglivy.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ypaflaaj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2hisqnzoz.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qszeerfm.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dpgopatk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2poglqrwj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qajivjdu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2yjrihcoh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bmpvfkwy.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vgaxuzhb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2daumfdvu.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2airgpntc.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lzmzpucv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mwipwmbj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qiqxnhqi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ltlcuoka.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2emttrhrq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vpdtietm.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jddwbami.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2tbhggwom.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uhfflbru.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2qybhbham.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cpqnpiwa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jxglyynt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ioaldahk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ygqbfcyo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ogagzzcj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2scktoyws.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2sfnaggwt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2hjnkkqnj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2tspnnkef.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2uugggyzw.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kdtclvuw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xwrwaoly.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2nxclnqkq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ouwtyjqe.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2scwpgnld.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ddbjnowq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rwwvezuh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ivariqrm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nlcfgmpk.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2asucayxs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hbzmhubs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2duaypcpo.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cgawiqya.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2vsxygjjp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ybjeuvlk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vtqtnflf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rvpffkxp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bkqscbxn.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2irzvdmzi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2pktksmxq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pgwmvjar.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mltdhqpg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ixluhtyx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2mfdjmbea.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wyachqnn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ibhjdvzh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2crqdmxfv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sryzontm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mmlroihq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2jnjrjuwo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wjarsusr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2tkfveawd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2znjaohze.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2atuwrjkw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2mqrtmsru.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2fiodhofj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2btxcyxmp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ewngytjw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2kebxwizs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2yytotsuu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2cvnhihxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lwhsgbad.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2rnbpyxpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gmoihcdt.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2toaqwmps.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ihzoeqfj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aunnqorm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iefzkdyq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxaqmrtr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2unfytjaa.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2khqyncwj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2qruzgqez.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynajkujz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fxurzews.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2rehtiajs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2pwudffuq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2paddsmwa.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2izavtmtn.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pdsnsbyv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2vulvsvnb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2mauszjon.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2drptidon.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2tmmmdana.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2bkdcwaby.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2nwtzfkfg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2adjylixn.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2limfpgoe.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ksgkqpcy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2gbhrmcpu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2slowcnbw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2oogjgvdp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2uvmjbvma.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2rocwnvnu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ybexnxmy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jswarbek.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzkhfida.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dsffgxhs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nhlceaad.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2suyqvtgc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fjzrakei.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2omxlytzx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2sofaeqcu.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xeowusat.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qbzvviks.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qitdfmcp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjfdtslj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2loxiedmx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2lfduliyc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hchdbtdm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2dvusmjiq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2jtqltgmq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfncjzgo.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mowlyjzt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eygeblem.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wccalvad.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2aulobxmk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2wacfcprz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2oaetcftk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ukpdvsif.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2xaqpfuuo.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pkkudevs.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vxdbbywh.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jtqcaytk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nrocpeiy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2vnkahmyd.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2kwwhnpjc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2dmanaafx.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2xtixoowj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2natseptt.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zztboymu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2kxwvxgas.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2nnaspayw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2bsjboony.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2rfgaalev.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2yqocqutc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2axgynvjt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ydawfjxo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2pxizpnxa.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2gktilybt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ewycrkhf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ddixxvqc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2drsszxib.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2owbxztwx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qndehqri.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2zwcpggco.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2mvsohgbq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2lpbpxcqs.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jvbxotvr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2plcdmbeu.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xewaqyix.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2nnpxcnbt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2rgmomqtb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2azhjbypg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2atwbfdbe.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2zugxsagh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2eegjjlcr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2czenelng.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2heddxdrc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejjnsfjb.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2shuebskt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cuwkpyqe.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2mlfbtuho.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2zoukdylm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2afoxrwvl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2pzduzbaw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzelzfdi.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rahejwbi.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2amdmqbss.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pnrgxtpj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dcuvkdiy.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2slebrqjs.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fyytneuc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2dghudulv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2qcchrvep.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2igkvvyyj.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yzfowgdd.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2desjvyxz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2evikiahb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2tgvnxynl.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2wmsszgmm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2wnjbmlcd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2aotsqqfn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ythbaywg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ihcigrsj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2bbwnitlk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2jkvjfjsz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cotbrrzd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2gbsfjcvp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2raclplba.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2zlonsidk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2cuqlfbva.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2uizvweoc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2lcwilpdm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ilqcfpot.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2aatmepms.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2vloxdbve.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2jhacbgwm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2azfedxyi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2inejtszf.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2vghlbuwv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2mdhsqpdh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2iikrfxzq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2sawcfwib.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lclrrrnt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2coinwebv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2xdmbmckl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2vuuikewu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2vokpkndk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nczzfdpb.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2gpnlpoef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jhvmxilh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2kmcvhnvr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ggugpsao.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lrxkzshe.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vedtzhiv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bifutrof.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2zmtqrmew.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2cntvzpwh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2kxevrxbp.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2jsisrxiu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2dgqondiv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2vtkgsllc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yxugzsmb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjeujxfl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uhhdnwjx.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rqdyfvfn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2lvjhovzo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ddxgzxms.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zjihvmun.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2mrauvikm.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2eozicipb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2htflnrkf.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2slrkmpty.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2enlytjxo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qjljxdch.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2izbzmbld.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2produbxh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zjkmsafz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2lsmymapn.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2trcgfnhv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2mvoukrmn.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2gzliywbm.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmomfazh.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vakqybhh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2ptfvogof.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2fkavmjvl.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2apzwpiqk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2wrkvzzys.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2awnfvwgp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2dltidwzr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2gnqevmzu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwwruqfo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nusitrvx.html


<!-- 参考信息 -->