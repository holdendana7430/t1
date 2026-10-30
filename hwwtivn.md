代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gtdmidzvb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvjynencm.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gqiigcwfg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkqvqguan.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwmoxkhpf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gizqlgrem.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gugdqewpu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gecdetotx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gljczzkxi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gcqylucsp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gcjbcljfw.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gslzusuqs.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gesqnpxdw.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gchqoehwr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gwypoianf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gxnjupnxd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gcqsfaqje.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gclituobb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gnaiskayh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gsgiglbhp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/ggbqjagil.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gdidfljrx.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gfncccpla.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gluzfdptb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gedppnziq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gvwznsdzs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/ghjkvodtf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gbmbkofqr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gjqsjmbel.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gqbdqxfsx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gryucmnfo.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gmmpvrake.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gthvugpjy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gpdhfcsvk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/ghbkbjrbh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gvslvtlvv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/ganatwtqp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gttouqtyj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gnvhbmndo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gkemksspm.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/ghrkeyexs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gfkrkcxkv.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gcnszwbhm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gciaozzsy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gytgtnpqy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gseybdjrj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gsvxkuxnl.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gobumcwgq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grfvptgvs.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gisjbwwmd.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyjpblytp.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gbpgekqpm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghmnejawt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gezkbnaty.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gtfuiniea.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gykjipxwm.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghisvpqwo.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gjszhbxkb.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gxcmhrqec.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gvsjbabhs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gtauoobpk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gaqrkusor.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gvzlqgdvy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/grrekilwg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gxtzomdqu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/geicoojns.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gahkpihvg.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gssfciivu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gewhrtvcr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gqoaytfpt.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gwwmxfncm.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/ggobykxkp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/ggamlntes.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gmnmemwht.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gigixwwnq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gkpkzuyvq.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gzbgrqavj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsigpnjhn.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gnduxnall.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gdbovfsrb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gmjjslgbs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gbwymcxam.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gwybymbtp.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtwjqvphh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gtpdwlekh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gwqzinyur.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzigdnfmi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gxqshsqkp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/guquglrmr.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gdgvqopfe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gganrazub.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/givazhqcn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gdcaihnwt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gyfbzdbxt.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/garemcuzd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gwpwdwhtj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/ggkacfrzi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gveudopii.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gysjvfwkw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gtnrigumw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gcejexmfm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gspgmdskd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gwqtxgitr.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gvazracfv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gnlbcyhya.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/glvblmjfs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gwpipatrm.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/ggbkutfuw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gmnfukzzf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gzwjlvcfl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/ginczhhxt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gmdbixelr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gihszmlcs.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/grftvmiju.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnwtfbfea.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gpmhfqayc.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gxjizsqbo.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gskaprhpp.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gsiumjjgm.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gqmrtplvw.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/ggizfuqej.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gpsyzexwr.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gbfpjutbq.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gpgqxzvqi.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gkjkzssgy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/ggzetvsek.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkbjssacb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gwvsunxcj.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gweqalzzb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtyldlztk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gpkkbtavt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/glpjfpsfv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/grrcmxjde.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gtxarhkpf.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gybvhfjzb.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/grftufzbn.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gqlvxwfwu.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gvacviypo.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gfwkvoyvv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gmnxbvshu.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gxnhxvjry.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gyfmyqfqr.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/ghjzqdgjx.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gyciiajdt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gskycnchh.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/goaoxfcfc.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gjksgpurn.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gipmduxxn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gysqtgdeo.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gbcuoxssh.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gkcmexnfq.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gtitqervj.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gfjokbcmw.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gqqnfapqh.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gnyoetkks.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gzoupxkdn.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gldqkwopx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gsbqffjhk.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/giwpbdsjb.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gecbgejyg.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gtxrrdwzd.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gajmqdone.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gaidcmtqi.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gpvukyfdj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gzjbnemcs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gdztdmynk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/glajdxkwb.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gntabiyzs.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/grkcidqqp.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/ggrtvjjqs.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gnqyqmsxf.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gvbwbtttc.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/grnofuzqs.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/glgxudvkj.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gdyymvyzw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/ghhhpkuwt.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/grnzpuvda.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gatocrdpy.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gaseclxje.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gurzrnkav.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggrzvfdsu.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gpzdzdicx.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gzmceeyle.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gxgoomxbh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gwypovxlc.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gimeapasq.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gqpqzrljo.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gjzpzokvp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/glodicdsd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gtzelzuyz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gmrjaoyyh.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/guvbbhigv.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/geoumreqj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gvewzvrue.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gwnmvmrck.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gzfuipywu.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/guvwlcuiv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gsacfhohf.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gkmjtpmtn.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gkngripcg.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/ggiorklog.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gqrjzytfb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gcpcmwpun.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gufuzqejn.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gwluoyidm.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gngkxsfdd.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/ggbwmvbyp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gzjqrqdor.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gvwfzhicd.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gfryamnyh.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gwbktxhct.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gfeiwwoko.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/guqnaomsq.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gecolxwjm.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gkinkrwtk.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gcasgxxih.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gpomvmssj.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gdcrzzolc.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gimyrjykn.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gdotbunnq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gpstwkrcu.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gltojbgay.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gbzjianqw.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gwoaqcadp.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gaidfemls.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gbopjchia.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gibijmqty.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gipakdyey.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gxcdeyeuj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gcnwmbrpv.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gwvqsedvx.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/giirrlzvf.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/grheabkiy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gianwcorf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/ggmvqcxvq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/gvgfwopoc.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gmxrfrvnz.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gnmknpjpv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/guwplsyll.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gvozssggh.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/guzaqjbee.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/ggnzjzvbd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/grtraxkcz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gflpovsgk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/ghzrvkico.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gsyypbpyd.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gotdnzvfb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gjoijufxk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gcakwtlwv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gybtdzjoy.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gtynjuzjt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gndawgumd.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gnrigbdsl.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/goejqkdte.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gerbaocna.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gafdqwcgi.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/ghqgtgeor.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gvoregnty.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gqmldonct.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjybevoys.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gqbhjywma.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkkhxnyii.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/grrmzkajj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gwitqhjif.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/goviuhuzr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gdozbfsqi.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gjytlkkuv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gnwhyrooj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gkmknmeob.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gupuaiosc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fehbvm.com/Article/details/gxthxytdk.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/glldniefn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/gwofdyruv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gbyrfhgls.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gqsabyhwk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gxwiebsyi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gtdaninvc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gbkxhlykx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gbthvjdil.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gxxalowsu.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gzvpohhqm.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/geohedvhx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gxjwnbgrj.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gpilpilqk.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gtofvioek.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gvugkxrlc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gtmfzzgmg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gkojatuaw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gfkryoimn.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gqcvdvzqd.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gugsdhsmq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gojargpno.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gyifqdkmt.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/genfwruwj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gphnwtlyx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gwqkflcod.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gactidqdx.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gjqarnxzx.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gfykbvaif.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gwwzplver.sHtML


<!-- 参考信息 -->