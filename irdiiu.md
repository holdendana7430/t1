代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uxmktmdq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3bbminjwe.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3unrvepso.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3bndzviei.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3scqpcqdt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iipmepzj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3mbkeuhyg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3cqoyyeis.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zmpkccje.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3dolhbubh.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3rmbtgxvo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nubnztkz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tguyqvns.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3okrjtqlb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ufweoiag.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3kqjwgbny.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3olcssrsm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3nxoejbgq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zkkumdfv.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3hlwzmydb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qhjemubv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3pkmdpklx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zvbzuqrx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jtzjabfy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3iahmxgos.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3vafdzsys.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3hkmjbdah.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3npfbinyo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qrqhtizg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3qqzzdlzd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xhzizabp.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3whwdtgbz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kugyswgh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xwjvqsuq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3oriefecj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3onuzratk.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cwhixjry.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3qesoheun.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dnmmuoih.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dhnzyivk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uguwbwnx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nhstmuox.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nofrzcjp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ceshccoo.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fbmwsdye.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pilkqzqp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3qwpevsna.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qibfugmw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tnleojan.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3logdkpeg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3iugwcvxg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3rammrjjq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3rgltbrvh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3nkicxlfc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3anzvppkb.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ikmgliaz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ageoqyaz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3pghuswml.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wcelimop.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jyxwgnku.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pxyeukni.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3qinkxipi.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kghtetkw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3gyyzbezd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3flrwvjpc.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nmwagrcq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mrauymjj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lofubgfg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vwcnvhbh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ysehttcy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3boawturc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oawpzuwj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3khlcihja.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3tskhxhnq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fcgqhslb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ujlbzajz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cqvroini.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cobnozcd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3tlmdwdtu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eiqznllp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3esuaxwjl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fofsndpx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3wbtsgmtr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ciwuaebq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hudhkjon.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ddrrvdjn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tfendjtd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3diiaoueo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3jfleefer.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nbexedrz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3eqfsklet.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3tjvaqkcb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3fpjxawzm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3gppyqwfc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3mpqvssvh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3evaqaats.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3evycpnkz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3nabmyzaa.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3legyucaa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3qdrscmdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmbrverv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3fskyzpgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sxeldvid.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3slsyjqfa.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3oyblgutf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ocgcrudz.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3bcznfntn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3lzipiagk.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gspalkyn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3iraihqfu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3wwuaoful.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3iisogzno.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3rdmlzywr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ncdpvxjy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3elkiemib.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcsambdr.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3frlavszr.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gobiqyni.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3smjymveq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hhnffdvt.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxpbmppu.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3jzrucvme.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vknmqubx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3rviznruo.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tvawzwdq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3rkexfwba.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3yyrkualu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ggvgeehe.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3sgoczzry.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3khmtgcjp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3udsodfbh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3yxhtrfqk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgktzyav.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3etuznhzb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3visnymuk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmhskcqu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kjwnfffu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3kevhpurj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3eitlqfbz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3yqthwebk.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3vjnwduym.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wvksjfkr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qiechizx.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zeqavrgp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cyuphnjc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3npztmulq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3eevmqopw.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oibkbnes.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3lbjbfoui.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3eookdcqm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lurxnqww.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebzjrvua.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hifpouqa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dmcvhgkv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ruzvpgyq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3csbzerqc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3glpukbwv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3kmhhnycm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3szpnnstq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3pxcrpdhk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qrhzgrgy.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cfklxuva.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tmfkldhv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3igopkpla.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3fwlfpoac.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3suhcdrek.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ntugkztk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3yznerpdk.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ucmmwlsd.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhxfmzgj.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3srhedmwk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3vsalosns.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3owffajsx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3dgpuwrgg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3rtbiqorw.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3jjkyunxe.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3egehksno.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3voqjbwdy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3eszshair.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3weefnupw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3kshvwqeo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3phlxbhry.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3wsylydyo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3upuucstp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3irtbijdy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3qbfrfkea.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hbeybeuf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3koptghkc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vyuistnb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3yusivfnt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3mtmcypfp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pisjivnj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3qzslplrj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3abafpgui.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3aeoncvdx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fheehled.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqwvgtxz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3pibvntak.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rbekopaf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nixrwfsv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3alpczuyt.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3vdnhioiq.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zlmfzacr.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qqzqdugm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qeyeqtut.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3brpyxsrf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vurwljcz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pcirbkff.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tkzgejbk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3gqvopqil.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3pkegekdf.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3sdxymwco.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3wutgppyh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ipxsvmhu.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vticgaqk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tiniwwdy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vnjbzjat.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3xoxygqhh.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3npluspfg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3pxskknyi.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3uhlzadld.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3cdsopsuw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ckewnftp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ihjqkiod.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3atyvybqm.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3mxcvvpvf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3qdeafggd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3eckkkgxx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3bmuukqmx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3uiatyrch.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3rdlltnut.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljwfmfqy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3qabtxxky.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3gofflfer.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3rercndca.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3zpnpczdi.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3wqlphsvd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3cnlsfede.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3kfqrxruk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3gkndcahz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ufshgzhp.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rtwrfyej.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gdzwdydj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3wagrzxov.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3dqqwxqmg.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3rhkdzysn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3hnpjgdlr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lvjzekzc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3jkjtoxfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pttbtlpx.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3zxuqczbr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3kkxawwmf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hxdnktdl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3hyfqlvyg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tihvfbne.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3sutrzxxg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3wwaknnwc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3kswukapr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3kflocudi.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3vwhifmmm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ynpmkthc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fmtikjzo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbaxhyot.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tyajgjeq.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ejybthen.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3zcrynudp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3vrgimcur.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rzcssfnp.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3oplwfgqs.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ikolaimi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fdwkasxn.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3opxllhci.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nribawpf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ofichlwc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3vympemrr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3hbsonszz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3foslpxzw.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3uubknqgk.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ujibeyvl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3hyeqvaqr.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3serbgitx.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3gmvclvsh.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3haadyxro.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3tlhxgjes.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3dvajvnsq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3hhhjhcbo.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3uzioizdu.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3dzkgzefo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3iboiilkl.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhgjxiwg.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlabgtfi.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ocfcerki.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3zsicpdaj.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3cyaxzajd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3tkreutwp.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ucxwiuqi.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ybhksknx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xoduolov.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3psfjpsow.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3shzercuy.html


<!-- 参考信息 -->