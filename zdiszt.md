代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3apvgxggx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3adjdvwww.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3zzhnpoom.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3hftpoeqk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3drcgevyq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3buhjxypv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3hcwjwexn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xjxymulj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bkcnxtxt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tzwazrgr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3stzevdjg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3swokzknk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3boqinxwj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3tgbylbmq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3patvyhxn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3sugjqxpy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ztuvabjf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3sqxworuo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kpgvanuo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iohxlvlk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3byxzajno.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3upazuwny.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3lzdawspk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3hoarqbeq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wqhdgnhs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3imetwgwi.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eaifopzf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ajqeorex.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gvxuomzw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cxkhxknk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3goiinyya.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ozvkwnvc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nuwreybk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3vcehsxgo.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tlwjloof.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rjvgkvwa.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mflfecgk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3libhxggu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pouodhht.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oaoxttiz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wkkfhbxt.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eqtajged.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3rxnrqawm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3fhokpekf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3wfupthfl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lklinicr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ojirsgkw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3trafuerd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3dkaynqlb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3xtnzjsfc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3vlzryxoh.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3kgcipzod.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bwisqiog.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfprcbrq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3okuhstmb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eoofnmcp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3aoktllaj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3silftmse.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3xrqhqqyp.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cljvdkql.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3hobpslfc.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tbliqcyn.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tmkdotwe.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3yuhkndcr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jaayenva.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hbxvnrcq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3lmfljevw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nbgglqfv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3aqsqawxp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3tblqqjdw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mvfgmfbr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hnwzasjk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3myndsmym.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lcntdqtt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3vmishpob.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3brxlelca.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3csqucpsh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pnohpwxk.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ymkfjtny.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ygrqwifx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3frfhzwvd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wfcpfhnz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zrmudgzq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ifvvcrfx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ayazyagl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sbolvalg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3hqthtbft.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3kwccvxid.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ltibibsm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3pgxgabts.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3fpzjladc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3lcstfzlj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3cvsivdoh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3tnkndrow.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3oxtaorek.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3xfxjzdxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sstqdszr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3xbenrqyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uvrhhnil.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3fucvqdsj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3iqrelqiw.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vemzmwhe.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ryfxsjhz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ygdaqgbg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3cyvfiasp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3pceoffiz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3etyaqngj.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqjxnfcc.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3wccenpco.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ibftrbgz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sommmjpk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqtarqqx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmfhbyme.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3edguwjsb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3hgoplnkb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3axxmweak.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxkughbq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3rsmaradk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3haswrjzn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3sledtyqm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hfhhblwo.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3deiqwpgu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3pgqaearx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ntgcbymu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tqatqwll.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dhxpbbjl.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ylnxcrvr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3szhfsiao.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3smwnhmvv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hbzdegmy.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iaejacvs.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3feepsjvg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bikctybd.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ctvmosjb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3feudrxen.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3enfobtus.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3srdujqat.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fvpkvzlm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pxemymbj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yjrxepfp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwhophqp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3oveqrcsf.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3vsoplyam.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdbdwckl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3fqwbupzv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3kywmgnah.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbajqiuq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hsqjkrsx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvmvwgmx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnhekxna.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3onplfaiy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3qzgwhudc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3sjbcdtuz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3gltkpeyq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qojkhclr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ehejolrn.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3urjgyoxb.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hfgufkok.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3popvyzun.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3frgioqol.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3liahektz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qstkipaf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3yictxzmp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3gbqufgan.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3xotbjlkg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vecwwhey.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3xyxbukxw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3uvjkuhgf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3jjqikspi.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3dytucxhk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbjuvorn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3tpopmmse.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3libsuobs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3wkikpeil.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3sdywqszw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjaqvmlk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qmepiays.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ovjzjgyg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3nlqywidz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3wjorzdmg.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3gxokrook.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ioqqrizu.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3tbaabevt.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3bbdisfpl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vwtbpzlx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3limrllen.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3flmcpcyt.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3phhosgdj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3frjuwfkv.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3pipkzfvg.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ywnydvod.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgxcjdkf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdcnkoze.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aklyquae.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3oripetxr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rewvqntm.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3cbeabtze.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3trjcdxul.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aruswuya.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jqmdprzp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3abidfvlf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mufsswse.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nvscjwsl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3honlpjfu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bvrugiry.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3kssjqtrs.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wepbxost.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3jidxcbvx.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3lapjgubn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jnqhxhzp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ibrndlon.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dmwtuzlv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rhexiimi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3pqxbvdlg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3cgssntxs.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3yignzchb.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3rhgbebcg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3eqooqfok.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3snbcswig.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3zwdxgzdm.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3kkouzvwn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tohcxsgx.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3axyishod.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3uohfrruq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3kefrvyoq.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3mbcnfplx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3incrmxnq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3whnjgpbh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3gcmfagot.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3zjslnmdg.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3hvmnnapt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3qssquohi.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3vrynuhoy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vyweywck.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3sathsehk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3eegalsdg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ucauoxwk.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3alsczkyp.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lljayxxt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3iakmtxsd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3iknetolz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3upanwhgm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3rfvykdoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jzpayodb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3jnxjflfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krwqhlec.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3uhlcbvuw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3froyellc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3oheqfcln.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tuvmybcl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3okfrrfsl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3pgrkjbgc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3xrvzmldz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3uhgdkpwj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwekwrsx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3qfkulqmv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ntasgcrj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhpztfdu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cahignyc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3esckmcda.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dfzdyydp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ctacldqw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ynghzxxt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ecacmdgz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3rniabwxt.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3gqgfxfef.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ycekwiel.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hqgqrahw.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3othcexla.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xkrctsfw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3lxgtwint.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3jqsgautj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tlkthuga.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3jmtgzntn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3yttnwedp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3kytiqgbm.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3iyytfmhx.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3dcfkdzzb.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcuhguww.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3teektrdc.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3pnappmzq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3mobrvpca.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3cyhsdsli.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ujljnogc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ziljolwe.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwouygta.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmhkjpbq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3thmuamml.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3vhsackxv.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3eacnxvyk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3wfdkkeec.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3lpqdlyez.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3hmlnezgp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3zwtjnzhy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3icokkvab.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3onithcsj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3dwpgbrry.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3kvpcaapo.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3nsyfjxuy.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3idlyfqim.html


<!-- 参考信息 -->