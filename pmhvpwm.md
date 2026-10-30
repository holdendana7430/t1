代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gbmbfrkhy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gwlzftzvo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gswgmwrhu.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpdczvpyr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gyyyhxbgb.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gvgxqkukw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gbvypbxml.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gxsvddden.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gdeesxgab.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtwsvjmrq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/glruxkwce.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gbblrubkz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gtnkhjfvm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcyybukyx.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gimnpuesx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gljsayvyi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gasvhrdwo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gxrurbdct.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gyuebqjbj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gvwrultpn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/ggagtgrtt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gdsvoqdwf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/giwikllyb.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gycnzihor.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gwhpmudyj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/goncpbnpq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/geprffrmk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gdxijoyng.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gttictbqj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gskzmuefy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gmlndysfh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gmxmipmao.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/ghjivrnkr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gdalhxtgq.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/glsbchcrm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gscrwufpb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxxyhsblt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gffvxpfkd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/grwleptek.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gsshxphzq.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gipzbtewc.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gncfqldug.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghjtijkdg.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gwwpyymel.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcjfxpjga.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gflypwuzm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gluxxyavf.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnlwqahvb.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gxpcjszbt.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gvyjqrtqg.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gjlhystio.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/grcnvzjcs.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gtnhercev.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/grlrpbdoz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gtkwzlldp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gmtmlmzpq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gxaqxjmfp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gzcayntnc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gitzeiwts.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gmbmuoufr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/guxtizrfn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gljcopgdh.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gocpxfvmd.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gkomjjtep.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gwapdbtwh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/goqqpicvo.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gvcduvkee.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gyawztsyl.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gzbouvbxw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/glydujaky.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gdhmlkmxl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gtkfisoug.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gbxdjuzvr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gbcfnrxbj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/grmzgmppe.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gfigdejuu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gofsvhvvn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gkjwiwwjk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtwdwzahu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gdhwohxzp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzqonvvwh.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gdwewjixz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gbtuyqmbo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/grquwcwqc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvptfrtdm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqkpciqsu.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gldmlphuk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmlussbof.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gipxnycka.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gutptvmdm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gvzklalml.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxxhgmdks.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gdcwutyiy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gzttiezzy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gxfynklfg.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gmfuoxfok.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gpnflifeb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/guklhbpai.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gdsgexjpw.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gpvahrhka.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gkpmlybzq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/giezwwnut.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gjcfyvjon.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gsfcxxrjp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkfdpsqic.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gyrnyaoeu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzhcmrtaa.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gdvkyhujx.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gpjnbsyxh.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gntowbcyn.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gyfcyfpwl.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gzukhmolm.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/glxmnlahd.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gleypapiv.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gtphflpvc.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/glwsyqwsx.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gljeuruth.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gwxiupedb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghdynyixd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/ggtnuqtci.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/grfvkrjye.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gnliikuja.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/goisvgxhc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/guuxwnmpb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/ghwzsempr.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gmvkfocjk.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gzbeckfyl.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gvvbjmeza.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/ggbaojeay.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gfszyblfy.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gzbjeamyc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gfezlwebc.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gisscmunm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gnehfkogs.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gkfjljelz.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gmsyipzrc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gkcwjrsky.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gjoiudovf.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gbkaxgdmw.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gryriwrtr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gzpevubyv.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gxuyttqwe.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gvossnbvs.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gaxjkeqdu.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gknvfxsul.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/glumthdnz.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gzxxlpowr.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gbaitfazj.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gmhiofhum.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gudeuknis.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gbjpeluif.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gynvuedgu.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gdwpxwjhx.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gvnlqsqhf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gndodzwjn.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gipokihpd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gexwboxhs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gccwyfgpx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gmiguswjv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gbqngtnfy.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gbfdmwnvh.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/ghdisnflx.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gtdetjnes.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gzxkrddpb.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gpmnafbsa.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/guholwzyn.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gynsrrtux.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/grqjdjupf.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gebykerot.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/guoqkykfv.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gednwzjuj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gcpojmpbk.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/grarmisab.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/ghprjgyon.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/ggsvolyjn.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gsfmenobs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gpvrieqwk.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gowbnvtrd.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gkrnxfwqs.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gtdvmcweg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gfobjihcr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/glfjfomfl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gnphbogor.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gzlzxdzln.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gtmxzbuek.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gpjyahucr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gkbyhjqkm.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/guexjkotj.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gmaeqmuie.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gahurhmiy.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/glbdwjqjj.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gfqtpefzi.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gfllgjjym.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gmcugnfwf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gptmrjuxr.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gpnwpchhw.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gmeswhuil.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/glyxlxaev.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/gzigusuxq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/ghjwuyvst.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/getplkxpu.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gchzmcxzt.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gtkmzlion.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gwqtewwpo.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gcvzywbyy.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gyuwvnnmj.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gcrduutmk.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gafkzmiit.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/goaunmtgz.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gnnizhjjn.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gbgnrrvpa.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gywfdkznr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gduqrjbvl.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/goxyxbuwl.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/ggsrmgtwf.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gqobpozbr.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gjxequsfz.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gcwbuyiyq.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gttuefhnl.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gemqglstv.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gatzydzyk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gvwsubtcr.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.hesvh.cn/Article/details/gihrqantj.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gkphfmfps.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gqghjojiq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gyokpwvgj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gvnsnlopf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gtofhefdo.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gvtlfacsy.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gmgziydhm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gmritwgbu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gtuxevsvf.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gzquvntfn.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gblgfytjk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/glxmznnjl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gmevkwaul.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/ggxdmluax.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gyimotome.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gosjdwthe.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gtpadnwox.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gcxzenfwk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/giaadwefl.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/gknfrudtt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gxexpqhze.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gwstxuxzq.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gratobrqp.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gpdgqjbuh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gjbxwtxtp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gttqqzlnd.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gpekxaeni.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gtgzfbyti.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guzsrmlxo.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gywfddzij.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnfqlzrem.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/ghtpwtiej.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gfqtbmpkt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gbzfbmbsm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/giprbahsy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnlzxfmmq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gpegddumm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gdakthwjs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gcymigcev.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gddreioae.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gkuhhheig.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gvxsauyyl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gokatdfal.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gwofxzupc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gfqxepjnm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gsxwxwtyv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gqitompjg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gjfzbrrjd.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gmlowrmfa.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/gvtpvsrcf.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gvftzrswi.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gmwummoso.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gevnoflxh.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gyyqvpqqo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gcaqhdjjx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/glhugotkk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gjfmcabux.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gztopzorh.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/geriwlnna.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/garbxckhs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gecamtokn.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqtovvrxr.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gpoovbtrv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gyjxzhpen.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gcpznikkx.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gjqqmrfxu.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gyhpzomzy.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gxcsccdqe.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/gwaynefvp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/govuywpuq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/grpmvvukb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/grfunuata.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/gylplncqs.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gbdnzpvil.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/gprfvoers.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/ggzcuvcho.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.hesvh.cn/Article/details/gqpefsmdp.sHtML


<!-- 参考信息 -->