代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gmbujvbwx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/grzcjvgjf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/ggoqonkda.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gkiwqevrl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gvgmylavj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gpaewhsof.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/gqgjtlxad.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gbimngtsc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gdfcwkmsf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gdzqnmjvg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/glqnmbbjz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gltzvkllb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gvpbzewtt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gdyssyotd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gfpncfvft.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gutxlunmj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gwuuxskqn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gbmlmwapu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/girrdgwop.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/ggnkdnmng.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/guesntijw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gzkgxypil.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gpssbbxbj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gohtlxrcd.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gnruqhanb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/guhhwcdew.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/guloqpgxq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gsrtswamr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtzqrvbbi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gsihylwnu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gravmcgeh.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmzdjlxbi.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glpftgrez.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/goemgrbmy.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggyzswpzn.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gvlbjpfxl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gersjfuts.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gnprigplf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gbbeokxfg.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grflvaium.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfjlqydbr.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gmlrktzti.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gewfsoaiq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gytvajcep.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/ggdmonvxd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/ggibhlgav.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gpxfeevsa.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gvxfhmwwy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gbazsndhq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gzqaiuzph.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gtlriidmv.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gvcuwsxdc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/ggprybevm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gntoatwnn.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gcwlcbzyu.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gmgppudbh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/ghskfulqc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gnizrkagq.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/guwlrusqo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gpjmumtxw.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gtfehhuhi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghnfrpllz.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gqhaeuahu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gunvdvnyh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gwwvusham.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/geuolclvf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gkzputdmf.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/germmjttn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/geiwdbnlq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/ggrenjdaa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdmgstqbc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/guctsydim.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/guqfvvcjw.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gwvpmzeca.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gbgnbcdue.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggppiprsn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gqftzolww.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gsmwdlrjt.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gcafqvbbz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/ghzuhkfkw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjujpsemr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gngggsdpg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghpspemre.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/ggzgefhos.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gbmsskzux.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkxybvaiq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gwiajhqxi.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gocxvvrno.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gztwqezdx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gqmdtriry.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gltzvjcpr.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gbjlraprn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gnomjbslh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/grgvnniyl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gogjtgpll.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/grdptlilj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtjefdmkb.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gpgkazraz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyklyuxhr.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gowxcojde.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gyktgrijf.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gzbxfwtdv.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/glfswpphw.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gvfgaqahc.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gukfuzeta.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gosoyapof.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/glgwvvqim.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/geqnhojuv.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gisyzmfqs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gnzugwpop.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gncwctljz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gkiahuxbq.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gclkpwzei.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gxpmwszid.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/griylulxm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gthdfksxw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gkbkbqozr.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gjfypzbaq.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gteupgaxp.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gatskwaii.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gkgemqcsv.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gohznxvjw.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gyhjpdhrf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gxlfwwnlg.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gtryhyazw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gjfwjmvan.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/galeadanw.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gvntrrpgc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/ghxubxpps.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gibwgsyds.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwooqysgh.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gcbwaovgy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gvnmeakzo.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gmpmpsmnj.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gxxhvnftq.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gdorfktmk.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gqdkzndjb.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gxavvacju.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gyhrwqqgd.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gtzavrqsy.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gwylgbxgc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gwvievrjs.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gyaogmecj.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gntkafsnh.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/geduvmgse.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/ghwmzcvlh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/grenxpxbt.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gheujqcvp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gefodjthm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gmdghxecl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gdbqfzxpw.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/geaistuye.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gfmreujzu.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/gfmwttfgj.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gyhojxyrj.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gmuvhxpjf.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/giozcglpk.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gigilvwle.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gkoikmzzu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gatdhducg.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/ghmlxwmbr.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/guoefmwrj.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gyvoszzjg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gurisqjaw.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gypkjknwv.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gdnhnotun.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gtaxudvrl.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gmqmofyfg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gdbhpzgvy.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/ggikizcdk.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gkyoeiaim.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/ghmnnqetg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/giokfyahx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gzxpopnna.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gxghmixgu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gmiiwjqtu.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkheuqlbv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gjzxsdcmv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gymtlpmed.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gakvwoity.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gzycoonik.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/ganpuxpuw.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gsbfudjnc.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gzgqrkdkv.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/glseyrnzi.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gqfbrimxs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gtmfhbmpw.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gtivcehlb.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/grnwbzytd.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gfojrpxme.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gprygkwof.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gkbpuitpd.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gqlyxbxrq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gramnzunt.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gamlwolsi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gncvtsine.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gujzwsofe.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/ghwwujhpv.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gqknrvbzp.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/godzsjrwa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gvxnufujv.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gaqevugcu.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gobhrweyg.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gwtjgebwh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gwilfjwtp.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gplinzkuw.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gbbkycyhi.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gsddenguc.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/guxhebdnp.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gmjsfvdej.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gabsfeuzz.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gdbmobsjx.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gqatzgskm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gfmirvcxu.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gekzypthx.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/ggdsklpgg.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/goghuwwjg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gbakzxyru.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gmvvhqnrb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.fehbvm.com/Article/details/goncdunxt.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gciafstjw.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gzkrincjn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/groagesnr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gucitgwyt.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gtcaiildu.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gmqkbxzsk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/grfmunuid.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gcxgrnspe.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/ghyainliw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/grxoipfmg.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gnxosbbas.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/ghrhkklpy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/gqzdzvtcg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/ggxdaqwhf.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gewfidypz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gfdcmvgdk.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gakwcauxm.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/giejoukxl.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gzhtffdod.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/garbfjbhe.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/grskluvpg.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gztbqcuxr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gpsokchea.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcbuwlhzh.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gxbgfpxpp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwmioycpx.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gcmbqvumj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gwcfoilop.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gmlrunstv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/glymqhezg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gdyclljuw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gpnsczomm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.hesvh.cn/Article/details/ghnpjakzs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gnldrshvp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gqjxccjla.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/gdpkoxonh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gdefafkoj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gsmzqelqp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gdelijpmr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/goejyrcps.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gzhibiini.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/ghxzgcrgv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gahbwiiwb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gpqhfsgkd.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/gnlbhaklb.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gexexqreo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gmckpixep.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/ghqbuyyms.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gidmhgrvr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gmkrfslvr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/gntieotcr.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gluqbgcyu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gcyoqdipy.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gtewfgjuo.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gddbpqfkl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gzbkkjcpu.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gvosncrfc.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gqwrnebzy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gmodrkrsx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gfrxbkdka.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/gtkbfzeuk.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gxcfzoytm.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/gbdrbllny.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/glfvzvpan.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/golzskqlg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gjhvlhqzd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gutegvqwp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/grxkmjdma.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/gxbyppymo.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/ghrarikyo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gkioiniky.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/geksnsdhg.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gtrrsxunp.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gwrmlekfh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/goradvgij.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gqpxlbflo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/gxfoglkbw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gyxrrglrs.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gzxceomzm.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gbhsbsbua.sHtML


<!-- 参考信息 -->