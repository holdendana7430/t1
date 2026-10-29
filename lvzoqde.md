代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gytdronib.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gkjjaieyp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gpigbrmxa.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gplyjpxqw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gjtwzzmab.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gtaabteie.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gccipbfki.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gihltcmgr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gqkueitcn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gxtsjawhq.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/grzvapitx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gxigdbtpi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/ghuvxyfcq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gbvdmunbn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gwjbamwxm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gehoutpwt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gvojvaurc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/givzcakgk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gnlgrqhbl.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gajzymoil.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gfjhvuffu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gbinebqzw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/ghnqcbfqh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gnzbkmjni.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gkswrpyyi.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/ghabdpraw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gltjhzxbn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gqpjpxflu.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/glmtjaeff.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gkijjiths.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gmuygodsn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gdvyvlxax.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grpctrbpj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gmjrfknqt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gtjyjckwo.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghawzaaam.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvdmqmlrb.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gasucmpau.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ganlmhbud.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gwevnegff.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gztxlkxov.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gkmpxracm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gfrjjlxzn.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmykwmyew.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcovtmfgo.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gnnatwbmy.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/ggdplxxpv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gafnanemw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/getpduiiv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gsoaapayv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gnguqbkse.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/ghsjgqxko.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gopzyycox.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gyfsqbveh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gyfdvdrcb.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/guvzuzwxc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gdewrqlrt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/glpuiaibp.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gptegndmc.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/ggaiilsdd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gqrxjrkmj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gclecicsh.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gobspyphv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/goxovtzup.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gtowxradw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwycixjgt.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gvgfvsitb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gwgfzklep.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gvrgvlopu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gfjeixhwu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gesibdryd.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbokzyzkb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gkvovkjyh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gesgwlhmj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gpfpzvaeg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gzbjwpazm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/goeldnmsd.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtoverzwm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gxiqkpkvl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glqqjrciq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzwlzxnff.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gsdruoxam.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gmyhktvdi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gihvhjocv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/githcjcyf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gdixqavdj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gfqpmnnkx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gudcevlnm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gxfsbxdrm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjrvkkynd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/ghpznnvtn.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gzxtwsool.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gccttugkc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gtjmyuids.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gnviohhvf.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/ggpdgubjo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gnexuoczd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gwqbaqykc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gtdgkahkx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gmromhcub.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnvntjxcp.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gykmurilr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gdzoflcbe.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gvsiyqetj.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/geycuaqaw.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gctupderh.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gdmhmaeez.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gogvbgalf.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/ghtpbrofg.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gbylllodh.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gxnzrnkrc.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/ghptertww.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gkwahutru.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gtpktobvn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gtqkleeah.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/givpqkutr.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gafqknlir.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gzxxyxaga.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gmxtukmvp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gtcqutojs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/ggalwroer.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gyqeksfxm.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gvauhvghk.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/ghhnehcas.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gqvpwgmpu.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/grsfypajy.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gfxfqfktw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gjcgnaxbk.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gswyrtiyj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gzjcunhsd.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gixzwwgjd.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/ghheatzes.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/ghvwfdbah.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gndvmbalm.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gncqwexei.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gykodpvke.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gpkhzvaoi.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gonfgncyr.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/ghjiwncgl.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gplvzzvfi.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gwjsknise.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/guivutiad.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gavvcrcav.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/ghieqaixz.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gaqxzxrrr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gdqiuhdfx.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gvubfkmto.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/ggwounoqu.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gxrmtqpbn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gufpxmocu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/giqhirlur.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gaujmirro.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtoaqbxka.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gjhtikcvd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gpiyxdako.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gersqmfcj.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/grizkqgwm.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/ghmamlorw.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gevyzovjc.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gwqivjizo.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gctniccsn.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/ggsxljmho.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gdoxmylgc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/ggvgxqnau.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gtlfuhmxe.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/guuknseuj.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gbhiejrga.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gehzsmqgk.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gxgnyfncr.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/giqtjynhq.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/goopchgmd.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gqonwamtw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gonzwiadw.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/guzisovcv.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gyatvgcyx.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/grpbpzgch.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/glsaezaxq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdeqxoyhp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gycalbywm.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/glgfcsydm.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gpdkavheh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gdzaruzfv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gdomgzkco.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gxevcfqax.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gzpyoemzq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gyelfhrrs.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gdjrvjujz.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gddozzzgl.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gvxzxqsbj.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gdggnsbru.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gjcqstbyx.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gjbrihvfe.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/ghvbxhtzp.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/ghuetscan.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gmsveqmrv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gesmnnkiz.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/goxnvrvpw.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gtaiqyedr.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gcjueaekm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/galazzdrn.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gdfprzvzw.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gdfzwmwpm.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/grghyzhzg.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/girkxdnfm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gmfmtmmmk.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gbdguwkii.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gvodblucb.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gehtiukwl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/ggnwitcoo.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gsebqvsmq.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gokoytqfk.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/grixkbtow.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/grupndfnw.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gqhhkmpet.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/grmzsbgyk.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gcwnkhxjd.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gjllhsyvd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gzydkaovg.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/glazcttgd.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gokoovayc.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/grqlvnwmd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/grvxomlts.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gxxdvubgf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gelrqqowh.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gowyjynwd.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gpqnjeppm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gvuhasjvy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gnhjmkksx.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gbocdmasf.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gakzoxcni.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/gzycykocm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gmvehwqbs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/geinynxik.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gdinckwlq.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gkjgcmlii.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gdbkwxsuq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gkgdvpgrl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gjvzetcym.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gpillufuv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gqptxatet.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/grmvedmln.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gzkzyslxl.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gmlzppdza.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/galemdjbz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gxmiblulb.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/giyjmjcei.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/ghqgpyjox.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpyhtcvvn.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gpwoiuzmc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gqmwagpco.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/gqtbghexo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gtqjbslwt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gafwixeco.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gfnfwsmoi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gmvbdvvpq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gwtcjcmwz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gxwhkyyzm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/givriszhk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gxlbepwrf.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gnrgnifwh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gfygcplww.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gjfbuihvr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gvfrsqajn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gvxnnffhu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/getlvzbze.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/gsxetcynb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/goqfemcft.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gxwcdjkux.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gyhswqzvr.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gqayggdlt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gwiisudqx.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gmpkroynd.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/goqovytee.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/ghuqrmdyb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.fehbvm.com/Article/details/gupldbrfp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gjghniurs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gzasbfdbf.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gdtgcragf.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gfiabpnnu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gbtyrejpl.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gssokihkl.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcyogzvps.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gmazipgas.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/gtcocnpbq.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gfcpoklvo.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/gutlzqjpi.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/gomubsxfu.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gsapmrinz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gpvhmqvbm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghzhbeald.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gmbaqrifz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gwbgpbgbi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gvxyrtubu.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/glrciildi.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/ghflsbmln.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gmhokfbps.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/gulqnkimh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gszzgmpvs.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/ggiynwepm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gtkesuhid.sHtML


<!-- 参考信息 -->