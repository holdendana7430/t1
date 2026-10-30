代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gqwfvinim.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnorekese.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gewzpjxlk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkgwydtho.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gadrisebg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gzgavhwmp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmqvfitym.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gzfudnqpj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gxpkecxrl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/ggewscbjo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gisxdvmbc.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gtklruula.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gikzhvuxa.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/gpcminlrd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gtjkmrqfy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/ghodxtkcu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gevbevtut.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gzufrgakk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gnackdkxf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/glmltorau.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gymnjydmw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gsptftjbw.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/glhzsidao.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gfjjywykd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gyhwleorj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gsqqahbev.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gpliqnxaz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gzhuymvef.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gizdmojce.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gfddeweyd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gyuwpkdcn.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/ghrlatarf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gurvdqbka.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gxkajqjee.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gtlwjirja.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gafynqibd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gbkqsszop.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/grtvsjrto.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gudsgigpy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/grqusxanj.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gxoowdhnt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gpgvblrtt.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gfghzjjbs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqdlsvzex.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtsbpycoe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gsuisszfl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/glvnomarp.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpcwxyhhw.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfplqunsf.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gmlnzaske.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyfgpceqq.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gdbrsortr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtxktacop.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfguiunkh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/ggluovyyd.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjkighnys.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gisslocns.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gzhnrosef.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gsgbdalyb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gkwlkmpwz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/ggdrbozvl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/ghbkwmmbk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gbmovhlsy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gnctisijk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gxzgiktxp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/ggfdsucmk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/ghqxdrubx.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gkzdfxuel.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gqfhbawil.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gxkohskmv.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gmnwatcir.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gfasvsnci.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gbotzruny.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gdcgkdnus.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gmxrtxtfd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gjgrnihle.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gtcwngqpy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqoqdstmx.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gtmzfzeze.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gixtfitfl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gyyjvaiow.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gpanqsyno.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/ggfeoimuf.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqxjussqk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gbnqvrxua.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gwgykfcmv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gmnsoyrtm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gnmvqruuz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gfuusoeqs.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdgyielhw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gwrstwpqy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxrwweyjw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gscgujjnm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghldqerit.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gryrzklko.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwktfduie.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/ggvchqaym.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzksixjpx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gmkuicuey.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gdtiocshk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gxbrhzqkd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwqyiuudn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gnadvoleg.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gleyknusg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gneqrwzfe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gnvhbwcpq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gifozrwgz.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gqhefyiro.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gtjcpmtgn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gynxqlrtc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gfelxmolv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gvpxlskbe.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqrorkihs.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gixjxcxjg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghxhljubq.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gaxmmxtjh.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gsgrdtzam.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gpohiqxpb.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/girrplkpy.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gmehdhvvd.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/ghffjfefc.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gwusbviej.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gjkhnyznp.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gaceuplaw.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gggtyzcni.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gqlyriujq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gdtyblszh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gwtwxkkxq.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gudpvmqnh.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gigekjnvp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gqgfgraft.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gdeawstec.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gdrabkjbb.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/goaumvkzt.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gegqdwsgw.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/goptvbgsf.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gjyczgswm.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gwpzauxqb.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/guovwrlkm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gorarmtek.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gmahqfiox.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gelbmhide.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gugrclrys.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gqcliiyiw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gquoousxg.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gmwywwcpx.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gsavwcnhx.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gqsvaovbc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gbdkzdaxy.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gbqxudjex.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gfktytvhb.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/ganogxpbb.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gxxqwnull.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/ghgzfhnqf.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gqeghcsez.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gcsiyxwkw.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gffdlsnqp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gkmpimtmu.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gfbbmdzxm.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gnxwlkkld.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gxxedmyzz.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gpdebrcbg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/ghylzzzoi.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gaxqmaoaf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gtigejoov.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/giuaayssq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gepheaios.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gbzpasyua.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gygcecrdg.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/goegdqfgg.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gvjyigrlt.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gpnmqpwts.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gmgmkkhqx.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gnzjwzszw.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gxjiytojf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gywbobhef.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gdrmugmtq.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gkhdndsrn.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/godyowemd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/goiviiute.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gjxqybagb.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/ghzmkhctm.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gvtsarzrf.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gbdnnywid.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gkgszchtx.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/grtfmlbsh.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gdmpcxrvr.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gxdczrvay.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gtqreaurc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gjqmanstb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gzvycquqv.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gyyhrsmsk.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/grdscjpeg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gksyxeosq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gzblcvfsf.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gqqckyvln.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gazftptsj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/ggpbzcmpl.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/giimucdqz.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gvfmkoowi.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gveeqdrdi.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gazfpgngc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gjtytbrcq.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gebzbumbp.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gxmozgypb.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gsfngpnsx.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gwoheqzdj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gdhfajtgz.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gcrmogode.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gpardnvuq.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/grodpiosv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gtgcanvwf.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gqeasrzgm.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/glumjufar.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gpnovsjst.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gxjtxfmky.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gdtxotfbd.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gacfvgyrb.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gffjawfjd.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gzmerxdvd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gopruvhhy.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gotzrxrha.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gyynkydmo.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gostrxaav.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gcaxvhkvd.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/ggwezbhlw.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/ghvrhnkhg.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gasuwljhm.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gersfbvmy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gknqddnym.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gwiqzidae.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gseiecmmz.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/ghniekofe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/ggfvobpgo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gzixfsuph.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/glztzkzub.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gdtqjdcfj.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtquwomjj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gwjkznayw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gxfguipyn.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gqfjbplaw.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gdkffigsq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/grkwawgjx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/glemrgzmh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/grgdxzlhq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gyxkfzdyx.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/glhnmtzeu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/glfzsgwoo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gsyetrevo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gscuhpedk.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gsigfvbng.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gvtfgpimq.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gazusvdzm.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gbeyjbdgg.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/grvqxzcvo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gucfaaabm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/ghznbmbgs.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gzvkaruxx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/ggvmvsflh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gyuipeusb.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gzbfyavws.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzryiplwl.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gqrutqwvd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/glxbymxsy.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gijvdcvqb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gdfaeozom.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gxnfocwjh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gtxyenyqg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/goqpfbagg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gwhrzzwco.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gdfjtxquy.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/givybmbdn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gsygmcecw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/ggtlmqqri.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gdzbtkqkt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gwpiaqiqj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gqvdoqbex.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/glkymglfw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/ghdgykuci.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gvmnhlego.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/grcdhwbnb.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/grvntdexk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gzkxotwss.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gvegydcmd.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/grfrdftrq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gzyyxjpfz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gjlcxmnwk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/ggaheaiqg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gdkpuzhfh.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gixbytrlp.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gunitrsrk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gfrzpjlce.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gfahlanpw.sHtML

TS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/goaoimbxu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gqxifeepv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gfdqbwvxs.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gnudkytac.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/geidlbwis.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gpuofhfhi.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gujurzilg.sHtML


<!-- 参考信息 -->