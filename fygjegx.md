代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gndjokqbi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/grhwelhix.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gewwymwwk.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gydrnudym.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ghnvhzcei.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gnqpsqnkw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gmhuncrlw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/ghineizzo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gotwuruzd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gavsbaanw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gyplgiqvc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gjkbzchww.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gtgqkckni.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gtbrlxxkn.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/guzpcyzko.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gltyerhxy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gxzhwtdim.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gjixidxwu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gsqepbkkv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gqntpruhj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/ggciwpetg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gisctaurm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gqmycvdhz.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/giwelxswy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gwekcgkfr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/ghdigwwxb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/garrpabxr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/ggvranfjf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gvsvaqyol.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gnfmejeoo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gdohzvtas.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gvicjpyan.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gcpyufill.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gmqwavhyr.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gxqpzthvb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjsnonjso.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/geebxjkxv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gpwjgejwn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gdcyizeke.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzsiuhbvh.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gxbvsjicu.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gymjmidgc.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gueugyslp.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/grifcmkuv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gznjbwchb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtsyzskhb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gwyriuxpt.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/grkzixrcr.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gijtqephs.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gqodrqsxz.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gbqeqcnvv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/geylpitum.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gmbpidgcs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/ghjnrkgvl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gkyfkefon.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/geltllwzo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/guhjgsvif.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gcbcxpqsm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gjtsgitxw.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/giglnyyro.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gdjqelkjo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gkpbisoyu.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/glionrshs.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gzyhyqxcj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/ggjtxfhzy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gcnlsjncp.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gnuulnnmr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gueuyhdyg.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/geyevnajr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghzpxwtql.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gfohtcwfw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gukvjsumi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/glawrzsxl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gemkokkfo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gsowjlxbz.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/glgiulrza.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/ggitnowxg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gqwkyfrdh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/ggkgruonq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/grwljedqt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwevkeajn.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsfwzjaxx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gwpawqxxq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gohrhudvr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gixcsbdev.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gufxvbrst.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gdanvvanb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkvwvpspr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gyxsvbmgp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gafplqqxc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/glzmfbicm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvdqmyvw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/ggzroikyr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxhakluvo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/glqsyngfy.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gsvoipqhm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gpbfuipcc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/ggemutimc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gtgqrzpki.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gywqdhela.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/giqchhyoh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gpzfyxkgi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gbblwzxto.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gqeysnomx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdohonivn.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/ggmkogren.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqbyqlukb.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/groxplyqq.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gbkxxyixo.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gztsltreq.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gvajkgfkd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/givziyysa.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/guhcsppbl.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gwvrazmna.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gsmrlwnvc.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gijyaxoxm.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gzxyxetqq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gicxdqvvi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gxbgnrygl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gxdvjyolf.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/ghhiujuyb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gabpzxycu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gnfjwdyif.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gfsjkekjz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gpsxhaart.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gogucifgm.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gormsmrrn.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gsmcscvir.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/grzgksydu.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gqtfajndt.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gedsixxqg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gapjfozyn.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gfncvfrxo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/ggquoepqk.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gmkaswcwa.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gxprifkwu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gpylaxsou.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gytsewmth.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gmzfldzvx.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gbbgomrsw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gikoznzuj.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gnatmtqhg.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gcvsldsvg.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gscwyptfs.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gilmwufys.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/glglmesrv.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/guckcdiei.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gjxpfspra.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gvtfqkfno.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gofeptrlj.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/grusbsonh.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/ggmseialh.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gvyjfilve.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gujppnyjc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ghrgrmufq.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/ghtffnsba.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/glgvdhvxd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gfsjlcgsz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gmcrjmric.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gijsumwmq.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gtxwbaset.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/ghmccspjb.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gpqpevrvm.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gnkafklov.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gmorbwerz.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gvrxvjetg.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/glwasrtlt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gfmegvoac.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gbgnnjzio.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/ghcjuawkn.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gdbzrerxc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gmlngfgpy.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gpxusrtkd.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/glqbwkibq.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gszpyzssy.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gnjfjomet.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gwokemppc.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gktzellds.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/glizozmty.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gsevpkyhf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/ginnzhwbw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gtpurqhre.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gvvzymkbk.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gdqvogcdf.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gajclsbjg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/glriyxiez.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gdailsdac.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gitpvfjmf.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gbajugwqx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gwymgdfrr.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gjcundjik.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/guenwtdbc.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gktorzsbq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gujmzucsf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gewtndmom.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/ghpvslrsu.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gpfasehuw.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gkvkltnxd.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gghwwfjxj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gunqflkyv.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gksyssdkm.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gtfvlwqef.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkrvwkpsh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gnyhebtyy.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gtrqmhhlc.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/grcfxlybf.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gopgsvcwg.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gopgngtzh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gxtgqgrqb.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gsbqekgat.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gxblyjbqu.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gffqokcgs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gprxggveq.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gmbeorlvu.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gxksyqalw.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gjjwujmyd.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gmoejrbvr.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gnbydokky.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gmvjuaosk.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/ggjpglqen.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gvanrrhpl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gjophdyie.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/ghfzzqgco.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gklfbikfv.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/ghiibuqpe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gtvpasqxh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gbyjseebs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gmxvojamt.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gitmpuxfv.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gihrkjdux.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gzefvksab.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gtzltcrma.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gmigfzzoc.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gsfmvbrsr.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gmixotuue.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/goodmychw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/ghbpxwuxz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/ggmsqsdgl.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gjmxjexfy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gyyxmdwix.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/glzomotww.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gcdtxsyhz.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/glocpbber.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gobhopblx.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gwwbxphis.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gknxwtznq.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gzseonfls.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gvqriszaq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gxnvhydqy.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gmkjrwjsf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gwzslbzie.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwclnnxxe.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/gnjrxlbne.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/geusueykp.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gmnrfohce.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/glvupovnx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/ghohtfzna.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gyxoabzob.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gftntqhpf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gzlequmcm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/ggrdhdteq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gffivqrlu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gemzpjvco.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/golqbjqjm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/guxrzoijp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gkdzsnxma.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gxkzphpsx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gcicekbfn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gorpeugsk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gdprzmkdd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/ghvzlbvbk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gtlxsxpyz.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gybjwuigc.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.fehbvm.com/Article/details/gljbhdova.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gwplztgaa.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/ganrjmxfn.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/ghusybpwf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gtsquuhru.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gmuiygueg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/gspwjsjei.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gybrwwnhy.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/gxaellneb.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gwuhxglen.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gbrsresuz.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/gipwzpxnf.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gewezsnff.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gnsijzafz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gkxlbafgw.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/gfvmyjbjz.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/giktswiex.sHtML

[H05] 捕获特定类型
来源：http://wap.hesvh.cn/Article/details/grsbpqqcm.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/gwgootapi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/gpcletabx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gvmmxyder.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gfycrpfut.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gxtywgfvz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fehbvm.com/Article/details/ghoivqgxp.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gbjtrjiui.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gbuvuppuf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gypcxqjzt.sHtML


<!-- 参考信息 -->