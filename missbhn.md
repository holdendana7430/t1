代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmkwiymbt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gxrzlylng.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gsxoukmyd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gkmsnuavz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gomaiwnna.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdtgenwtj.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gqcmaojeg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/guhdbdxii.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gcqyuxtkn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gdfymfhoi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gvjdalito.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gkfbuxcbb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gfkonvfzo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gmpgqswtl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gnjtirqdi.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gcyydtdck.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/ghgxudhyk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/glpkypjux.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gxawvkihx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gbdgzcbct.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gilblmcbt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gihmwsulv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gjojentqj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gtmyjxbwm.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/guvtgcvhv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/glimuchfu.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gkjnsewie.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzyzzjjjq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbbcbattq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gpbueufri.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gimippcms.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gsvscqsut.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gxgueaqqg.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/ggmyxaapu.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcgeozphh.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gwrazcxyj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/ggpppqyxb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghvbobfjv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gkrydvghq.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpuncmdma.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gywcwaiap.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gpzaiitfu.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gykwxhhmn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/ghfpqidry.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gnskwspxy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/glzsjltqn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gfevnelwi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gjyhwvquk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/ghvebbcvd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/giptkzpgp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/ginmgdwoe.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/gtaqiuini.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gsxvtjkie.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gbhuuwfml.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gxjdbvucx.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/graazkcyw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gyeykdqmo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/glpmwjmnq.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/guyfgxovu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gtvuywnby.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gnhlfwmvm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjitwnnrl.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gxysqwnec.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gouahrgek.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gwqprsvmj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gymkdzzes.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gaitvgjot.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdjwztlvo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gfnuzdbfm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/grwcxzccv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gazzeyblr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gjfltmsxo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghjqrlvhm.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxmlgilcs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/ghffxnvou.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvlbwqakw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gkfiyqdwb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxuhsifxd.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gaecjiuiw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gjbtrdtjt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gmbogptdm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gyvrjguna.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gdxxbungz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/giydqdxeq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/ggfwmdwxi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gxyeehrmo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gpoczttpg.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gilzvmyfq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/getffsbds.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gidtgyygf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gyjdvfiiu.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gponqvici.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gwfcciqwk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gijjbzsql.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/goidxtrvw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gxzkxlqjc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjkgbakog.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gxhwjuquw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghtqymayy.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gwsymypyu.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/ggmjsdhfc.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gkckmfcqa.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gotztlcie.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gnotaolnb.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gonjudbul.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gsuzfgcip.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gdwuofcwv.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/ggsjfycze.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gacdmetev.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gjsvajstf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/guscepmaa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gpjzdceet.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gsxmrzyyw.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gtcsnigve.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gashxtryn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/giysshwxj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/glvbtmbes.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gynklvfcp.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gcqzrddzo.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gztmheczb.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gewismuvd.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gsswjqsmd.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gssxwgnfx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gdfhytcij.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gveggnrdo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gprfgnodv.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gsgaaslry.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gdncywnyi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gucbiauas.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gugsxpesw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqowbfalx.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gdhreushk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gayzshwak.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gnnaefwjx.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gtidslnnl.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gqspynxfd.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gvgczndfa.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gerfarsoz.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gimlylshb.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gziwtpmih.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gjaitpbwy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gtpvtlzbl.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gmztuwskl.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gglsbxuls.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gtblkyoaq.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gifmbhwaj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gfthvfmij.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gikvbumwg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/grncxvjev.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gtfnrioxx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gavttxbms.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gccmqgivx.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gpzbyfhkb.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gtfdhmrvf.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gqvhsdkij.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gehhaexve.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/grniwrtmi.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gytdfffpi.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gzonqnawc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gdjmqwizs.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gqztzgtln.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gjmaqhvok.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/grduygodt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/ghiafyhga.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gbwtmiafe.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/giirqdiqv.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gdkwfqmsb.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gjqqusuut.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gqvvcluyc.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gcvibceiu.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gkkyxeliy.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gjxpcxqki.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gbpcnrvcr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gcsvskeas.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gqyynbuop.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gnasterbq.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gpidvdfxr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/giyvjjybh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/ghfpwfgfn.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/ghpeuekpy.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gnbjqxeqo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gagjdzfxl.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gwyrpsxwz.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gewcjvcfw.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gjfofjoba.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gnkgsawlf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gyrqssuru.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gtwjtzpci.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gemygnfcx.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gugmakktg.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/girsbixju.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/ghhytyzmi.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gbjfuymke.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gkwodrvvd.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdhmytdja.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gkrlfxkex.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gtdgslfdc.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gurocwakw.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gsctoosnm.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gefctnrbs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/ghuouvmye.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gitzluxqg.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/ggjslrnim.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gkcorgzdp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gakynuuoe.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/glygxdvie.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gwkqpyxwa.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gluvrlqem.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gjnujlnoj.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gkqhprtyf.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gnkebsfdn.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gzmblpysv.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/getpvlate.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gmbzfgjuz.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gkeqsrjxz.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gzkuyvkyl.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gijirspoi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/ghhhgdlps.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gbbryarnl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gxhjaivsw.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gyvafyynr.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gyakjxxrw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gihdjlldk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gvyyvrmnk.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gxwanmuzc.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gqcbtfgqy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/ghdcoguil.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gcgvkmyqv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gomuekwal.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gymbdozje.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gluiusljj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/ggsobanwi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gborsvdjf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gwyfaeaac.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/gogpbeira.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/glfbbsidn.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gwgsssfta.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gfsmcmiip.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gqnnrbalw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gdiqvdwgc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gfkrxpkks.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gsxjowfmd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/ggqjiwfov.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjysfvqwe.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gqtxaecuk.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqiihngdu.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/gfisxroqn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gdohfcvci.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gdahcgjvc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/goracxoks.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/glcojfxwg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gmepbsfbh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gwcxwsqzo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gskzsefyv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gpiupsqsw.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gwfdwomal.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/gabguoexg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gkfhzubfp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gftqbktpo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gqxgoowqz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/ggsrdazjv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gltrhzufz.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.fehbvm.com/Article/details/galdyvnts.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gmzyodofv.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gwhpmmquz.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gqaohzstj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gevuysdvz.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gabjbfboq.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gbqqkhops.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gbdvubikr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/geruutyuz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gevcabvnp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gmoyhbmeu.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gbwgvuloj.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/giokpyrbs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gbcjwbiee.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/ggkmwhztz.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gmpjumuof.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/ggynflnkz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gnqabbqxt.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gykokvthv.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gczrhtlub.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gvuttpizd.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gklsmpsgq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.hesvh.cn/Article/details/gogdootef.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gpzysznck.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/glazanhcg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/gdjuqxvmw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/gigcjiyco.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gfcndplib.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/gfzafspkj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gxfpqrsjr.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gjmgvixvz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gccstilub.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gphqpruza.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gggskhmmk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gpdtzccvc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/gpgzisqnj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gttvarwtm.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gwgmustjb.sHtML


<!-- 参考信息 -->