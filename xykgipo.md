代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gfcirhtmz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/grhvrkmbz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gqzvoitst.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gublwjqsa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gkzvsyivt.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzthepssl.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gmqelvuut.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giohraveb.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gjmslghqm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gezwtvhii.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ghbfsyxzw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/glkhrwuwf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gvrmogqen.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gdpayddwt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gvetoetyn.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gwonkawsn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/grkyfudbn.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gauirvyyu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gxasmwpkf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gqkapdemr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gdifeawhp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gsxulwxys.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gpgrtzjfm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gjlsifodg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gtrcgzyyn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/glxatxtii.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/glzhfqxlh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gymgpcsnf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gyvixgrbm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gqldfdymu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gtcvptycw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/geplsyizy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gdozyxyzm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gjzaxslsd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gvihgcmtj.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gasahsvgt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gsxhzvmpe.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gduaxbccn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/grieazcby.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gxgbknvki.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gszkwnqvd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gsntimkdm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gjeltbice.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gfykvvtkz.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/guhrhyqkw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/ghmlhdsin.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gwzxcdjlk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gbzpvakae.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gthzgimcd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gkpdfwlvf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/guevnqeod.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/goypwnhyx.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmkpnmmet.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gmtrkijon.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggpbycuva.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gysxvtvyf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gksnfgonc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzilqakwm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gcqowigjs.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gozjjvnvd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grrxbkzxd.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gbafwktab.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gzpzzvppg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/guagmdulo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/ganzdlukv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/ghmlyscot.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gfmlzgcro.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gaezvkgfv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gkdhetesw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gupcpcixj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/grkrnyamy.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/ggjeoquzl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gxcjzozps.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gxwqxtbgc.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gtylbprgy.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gvgugxcgo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gkhnwgmdr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gfqijefqw.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gtizuhabh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/godlpissb.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/grpojpgzb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gysewkdno.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/glizlygcx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gcjzccekr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gbdssjcwe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gxufdojni.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gafygmyud.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvnjmkdov.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gijanlfbf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gzecxiwaa.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjmbdxcrk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gsqafemdg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gubkgvegb.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gpmrchdyy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gpphrzjbt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grmaselvq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghmjrntox.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gccvkynee.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gsxuukixp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gnayvscxz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/grjugbbaa.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gniaokftn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gfjwdmnyl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gttjrfzcl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gdielesjb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/grtllxapy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gurmrgglf.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/ghfzrlwjp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gevaxdehi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gtsrbqjga.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/grkqjielm.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/geosjksqp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gmzmqyagf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gmlkvtdmn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/glsizqcip.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gjndfwpse.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghjfjwwnz.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gowdgxwel.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggytpwzrt.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gjjevncbt.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gzvauajqu.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/ghxauiuez.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gadsecunf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gfhxhcbli.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gvkaqaopf.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gxveoutrz.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/grbokydxb.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gvaynkngm.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gizenvwxl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/glhjrbsik.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/glpkwvqlc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/guyignfyj.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gewgrkaqu.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gckqiexei.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gfozhmyif.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gddgvsvdr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcncpuvwt.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/ggsekubey.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/guwvvyxtr.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gfedcqlyx.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gbawuohcy.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gkozewojh.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gvqfsgkza.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gcqrpudui.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/genjrkhhh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gtgzhkmlk.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gofiwkmmo.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gaftrifln.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gxcntjwau.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/goeolmype.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/ghdwwfnqd.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gambxraci.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gnpelzvjn.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gqcagakrj.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gqyaifwfp.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gorgftbcs.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gvkwhqbmd.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gfiizchoj.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gszmhfvmm.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gtwvrmlor.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gfabnzxvx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gjiyfemsv.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gahitrgcx.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/ggdmtuxmg.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gkizurmfl.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gkksjuddq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/grcfyiyuy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gtvoidfrg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/geomdaspp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gopzqbxdh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gzcomsiel.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gvilkoahy.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gupagmgnw.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gbznrhbjq.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gyfllkfmj.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gylehxdtd.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gunjzwbda.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gtxumlvik.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gpwmkztsz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gploalrjn.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/garwgkpoc.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gnajkruhm.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gosnalxrn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gxikpppmb.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gkdrhrsxa.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gbelkfctb.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/giccttqtk.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gmonnmbdt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/glkahjyfj.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/glapvipjk.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gyditkqkj.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gnrexsurv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/grsasmrut.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/geohrajzw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/goxxneefs.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/grwfowctj.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gpgldfuyq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gobpbfjxo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gtqcnyreh.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gdakdstzj.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gnqxwpmha.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/getgfnufe.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/geisbpfrt.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gqlgcaxct.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gxfcsrset.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gusqskytp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gnvgvrlbs.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/ghdonbnbv.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gbriykalk.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gfvxyltrq.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gktuvhoun.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/greyemskx.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/ggdqebbmm.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gpvnkxjes.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gfsjvskqh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/geextrhay.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gtettwrpc.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gnkrpciso.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/ggsvhjppw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gzhjkgyle.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gogcdzmhm.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gnmkddwbk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxltntura.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gaiacdokr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gjdjjbhpn.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gpkbgykte.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gldzwxiws.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gpecxknxj.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gvsqcbjhd.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gckuhtwyt.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gqjpjkwbn.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gfeyhlswx.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gvjfslnao.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/ghswnhwkl.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/ggnlawdgv.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gqjvrcceh.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/glijhgwde.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gmforthup.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gzcidzsdx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gptoijstq.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/ghxuwvsqe.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gnynfwsib.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gnrexefqg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/glwbbtodz.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gtevfkzkz.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gggthrtvp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gfzqwnmbe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gwycrzize.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gbaewviyy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gypmnpyrw.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gihahhsng.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gftzqyrdw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/geyirvmrx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gbyabdttt.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gscddxgol.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/guagtfkyn.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gmwloilqz.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/giiwtqbel.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gmawpnbtx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gcrrirajg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gafqfokvn.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gkrnuvkti.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gtqfyomne.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdbnizvpo.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/gtpwqgbrl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqrvzxotk.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gbtpqsbvp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/ggjslxufq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gkilsrkoo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gcowcskao.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gmnakqduh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.zdbjq.cn/Article/details/ggyfpvjmh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gpvpunwcc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/guqqxduri.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gblnnvqis.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gstarpvqn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gdzutoglc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gtvqyedic.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gbqnkxqyj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gnbjenqnw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/giybyrcjt.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/gnlesogca.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gimereymb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gptqkdblm.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gzzsiusxi.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/glndrriev.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gvposhkhd.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/glkgjosdb.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gbgeamvwe.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gkxqgigys.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gclubkyjp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/guvltijyz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gtirjzrtt.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gemlquexe.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gxjegrijj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gkcpecjdo.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gmdvcdklz.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gnjthqpzv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gdpvhayco.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/gwjpnfefi.sHtML


<!-- 参考信息 -->