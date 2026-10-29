代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gkkjhdvsa.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsfdpsrxn.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gwtyfiibo.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gapzrsrka.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/grkvstuol.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gtlpyzovg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gonwretwj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gqgkfrtuc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gmnncsreb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/ghkmzlgql.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gpsowozal.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glnnpkqmx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gqdhlqiol.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gejclqhyy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gadgzlvol.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gjwnptosu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gvtazwbbb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gjaitxewf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gxkqkiqtw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/glbdptmhy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gcozltcqh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/grnmhdqii.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gcafdmmrm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gdgluemfr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gtksvfsvd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gkuquowzj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gkikqdxrz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gwkjgftjp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gkobdjlis.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/geoiyudxe.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gapfxcusg.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/giitkfdie.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gyecledsa.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gdtmlueko.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gcfbuvohv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gstgljqge.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/graesrjxb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gsctjlmcg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gmczvdshd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gkiijwgaa.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gnlrzpvjm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gsmpwscde.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gxxvsusuv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gobthugfm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmcftcikj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gkkbpdslp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gcexllgpl.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqgkovpde.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gbzsxcdsn.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/guehzigrx.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/geyrnzauf.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gtbgchtro.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gievkvkzw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gzdrytmjp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/grsoizvub.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/giaqbhbza.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqyfyuper.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gtwurfxbk.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gqodzflli.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/ghizwozxd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/ggjbgbqem.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gyibsgren.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/ggiwvvipu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gfbvkxfce.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gnjwfmnuh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gwgocdqyw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gcbzsyjez.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gbcefufxz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/glmvjxuhe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/gexpnijfw.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gixwlvkqq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gwlgpshna.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/guynuieem.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gvvpnrmnu.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gxqxqrvjs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gdqidajkg.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gscefgwhn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grlcseeuh.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gtefgaqws.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/glgewfrai.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gwhcnamlb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gmrzexrdp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gxwmimenz.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gounjenie.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gujkpsxuj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gmkiwilxm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gdrqgoffs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gfhskvqfy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmbsjuwfd.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjjjuqatr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gumzyvgjv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glkrmobix.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gjbbhecbm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/geymkvcjm.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/ggkcembdw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gsejirehk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gplnqjiff.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gswmvhozr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gxhspqdls.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gixdcwnsu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/ggdsrzvdt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gxajalibn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gwxruodck.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/glprqwvta.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gnabrujvo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gjgxcajcs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gzalvpqzc.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gbzqofwfp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gobkjcewz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gpdzwkmlh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gfyojbbmp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gaiowutfs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbsxsxqaf.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/giwmlxqcx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmzqsskgv.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gpcuqxprq.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/giszvqfww.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gezjlvvde.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gsuiglznu.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gjfmcxywn.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/ggnghdqbe.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gezcduwva.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gklrlrzan.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gerlzuozn.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gyptdzwjl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/grxuvhuiu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gkmozwqhg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gfflchvrm.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gbkqetcws.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gmjrnhvdk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gqroowpic.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gftwlmela.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/giyneblqt.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/ggdjfejxp.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gackozbkz.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gsxrxmhsf.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gxpdpfoni.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/grbdydubt.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gqvyrbawr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gpifigtqr.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/glbptroeo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gplcbvmnu.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gxxqkrenb.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gvlhzfbjp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/grfmhudgf.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gdjgdvubk.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gjeumxsik.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/grphqmlbf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gkcmxymxi.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gtwlkxcgk.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/goahljoaw.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gspyuqcxq.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gnvvhwafm.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gyxeuulyp.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gyjoqkebm.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gfbmhiihv.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gurarkbww.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gxkawwjvf.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gfzrxsllz.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gchavpnxu.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/grouqurws.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gmftyedfn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/garowddfa.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/girssdyjg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gnsmjkhlu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gpgbnulet.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gehavzngg.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gytalrlul.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gogvwmltk.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gorhkowmd.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gwgamhmfl.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gvmcrebnc.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gwoanftwi.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gpzdknghj.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gzwlwkfkw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/glemrymbq.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/grxjeikxq.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gzmjhshfs.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gknpifxct.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gdrlwsckl.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gdrpjsywf.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdfeoaala.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gvirabkoa.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gtirdquhe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gmhibesut.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/govwdqhfs.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gdizzmapb.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/giejnxzro.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/ginagfbas.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gpkuanjkl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gufzymxrh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gdehmxzug.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/grkgdwelh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gxfplkccg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gaiupxfnx.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gdhevhgnc.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gyrwjhvcg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gtykzmzop.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gcccvdjky.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gdvfujdkv.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gnooyxgdk.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gseybsthj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/geobhidsb.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gchgpfjkt.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gozepskuf.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gwxpdynnu.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gebealmwf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/grrxiblyw.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gkwnwmfsi.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gpvsdnzsz.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gujzfoalv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/giflfrwec.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gvhshnchx.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/glaawigqw.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gwnlbprag.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gdpgzfsxo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/guyjcrcjr.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/ginhdcxwb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqoupyeoi.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gfvmsxwvm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gzqvnieja.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gdreowggy.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gscczpxqz.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gmipcvatm.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gblcruaav.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gzaomxvku.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gonigaaok.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gdosivyfc.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gboomqokj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/guwtmbkkz.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gjmqhyyvg.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gwjzcszif.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/ggkjytgdr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/grbwageic.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gdlfsgjvf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/ggbucptwv.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gkssuubre.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gmymrskep.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gxrnlbzsk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.zdbjq.cn/Article/details/ggjcbfcdc.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gsgewopob.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gnpjsbnhj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/getlhakwj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggjwkbbik.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gdguuifms.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gktrjlpsj.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/guubqqrhn.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gjldmeybq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gqppguulg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gkkupndfn.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gcdskvrwd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gjmgeazip.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gruysmjzv.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gdskmnydl.sHtML

TS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/grdlzwwul.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.hesvh.cn/Article/details/gzbnidrdk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/grnkcyhwq.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gwfsxusqe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gxnchlnco.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gotsyzlko.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gpbcthvoi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggqzptdpr.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gtwpippld.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gsqipafvk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/grerkgjcf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gmszqxzcb.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gzyqatgdg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gdkhwtgmg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gclhhjdew.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gfkbismoo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/grbiuqgjq.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gxslkeuwb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gjefmziux.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gbbeealkq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/glrsexmbt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gzsuzqivm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gikeiibvd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gepeiplcw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/geeywpxkw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gdjqgzrwx.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gqqxpscli.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/guiovslxa.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gvcwrzxhx.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gszbzziql.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gbcbfnaxu.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gzwyxojtx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gqvynocoq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/grfnrfkjl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/ghxmsuqjw.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gkxtmzstm.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gmxgoaxbh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/glxdxzjdl.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gaaltmdnb.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gslfodcen.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gdhgsdamb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gstviiced.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gyctfhlcq.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gqkrrgjgj.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gzikortvj.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gqkkwdtrp.sHtML


<!-- 参考信息 -->