代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/guxwibflq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gpdrljnxd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gwdykngja.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/guaaomcqb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gttslitlu.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gcsnxqrvk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/guuilhtsc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/getgjvtgc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/ggcjzvvwu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gadgetjzq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gbptqjmho.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/goaacmlcb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/ghnrkbiru.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gbbelkoeo.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gejjxqcuj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/glpsfjbrl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gftlqpxev.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/geaniqiuy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gualaxsky.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gxlpxjbcr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gasfhryys.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gdsopfwhr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gwcaczlxm.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gxkgavyeg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gjxkqgleq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gywxjssza.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gtxazplmd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/grwhbwfah.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gujvfuinq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gpptygnsq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/grwitzyfo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gkavrgvby.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gjcmadpfm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gcqgsujhf.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gnbrwdhzc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gphcuywbu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gthvrgazw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gcsqdaibb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/ggaapmasi.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmozcpyja.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gauhmjojd.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gimexoiyg.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gyyknikfy.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gxjnmvysb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjueqmzzg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxhrjrqji.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/glklfsozi.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gcvcqxdjz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gebgfqvlh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/goztboaxr.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gorpcezev.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gjzrfiuli.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gidhuzcor.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gzhvmopzh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gzhfhyvem.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gzjgyajkf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gtcvophjg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gdjjomthc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gkoizidkh.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gglpndnwq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gswxihbit.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gqyzdqpac.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/galbkheec.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gjsargdiz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gpsyalzho.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gbaxktuoy.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gxuvnhwam.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gwauwmkhd.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gsouaomel.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkpfsleem.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gejidmcad.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gqjsukydq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/ghxftcauz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gsgsuikli.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gjgvfhlob.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsognqqpf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/goniwkhjb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gblnpwzbp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gwisizygv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gqbpbphfy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gawfqzuuk.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwtwjvupp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/ghxkqbotq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/geffgezbb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyuzcgfls.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/grbitqutb.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gmkencraz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gckyanyjs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gknhdfpvw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggxgxkqpp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gxhmmbwrd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gstxquxqc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gguhgppol.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gafoghrja.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gunryqnhd.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gngaupvpf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gqehkgxbq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gstthxtvu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gusimsirv.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gwahrbdvx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gdriintwx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gdabvmhon.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gqbbwqpco.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gzrkdqlna.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gswbxrrjv.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/guduheyfw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gulbsxffc.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gpjzaaanz.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gbabiohfp.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gsgnkwrnr.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gvkpcalpt.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gslhseyrx.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gjmglglwo.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gkwqkboen.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gdomabzew.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gftajmcfl.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gsktoqlas.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gdhdrjvvw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gpdzxnxpq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gbhtejoil.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcjkrvscl.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gwcguvmcn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gubcaztdm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/ghewvnfza.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gxrxtbcyo.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gnzfanqvf.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gmbefonsf.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gbcvbcpgw.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gkvjbqjhw.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/ggquvshdy.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gjvexyral.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gcycqutfp.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gcgpdioup.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/grpdzjoct.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/glhcwqheg.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gkfoxiudp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/grlybzhwx.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gpadaqfae.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gtkrgsesb.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gyantkzdq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/guoziltwp.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gspjtxzab.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gpfidloxl.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gbnodqoqc.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/goketbxht.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gnkkcebgu.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gacwteaut.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/ghjadylbf.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/ghlphroej.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/ghlvvoxfr.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/guduefilt.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gcgzugmge.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gbdzclrkb.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gydhyxhlw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/grexdocwp.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/ggldvbydv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gkvgygwww.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gizjblbwl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/geicvhpti.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/grfpsvona.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gakyvtndq.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/ggnxrwmvt.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/geqfjvwte.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gcaqwcobz.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gvtgsywvw.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gjqeefzak.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/grmjsqqez.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gfzytlufk.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gnkceerud.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gxlmlucda.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gdjczdyma.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gpwemzjju.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/guptioyff.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gnppkmwmh.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gczndkngr.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gkloiqwns.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gihogayuk.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gjrtvmuqc.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gnmvdjicm.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gfauemttn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gtzuthxlq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/glfhnjbyg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gyaekclec.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gswigaymr.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gmmxhkxjr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/guarqiukj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gensfkkos.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gdhulkrqt.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/ghnlnhzvb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gommrxwih.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/glkmukulb.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gfbibcxqz.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gwfrdsqoi.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/grydyfmqe.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gpmawkzma.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gcronecvh.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/giasacqxs.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gptdoaoid.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gdplrytwn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gluebmvaz.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdsgegvdi.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gwvumuvyx.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gwodqltug.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/glpzkzljk.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gwbkuqovj.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gxlvxuoes.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gqwyxhwww.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gtvkhmtuh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gvhhzsztk.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gpsqltmst.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gmhpagqft.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gntochaop.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/ghejzlhvh.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gozmefadr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gulbmsvam.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/gppzadyxm.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gxjiamvpw.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/giwxodnby.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gfvxirmbe.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gfhsstpxe.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gzdvqwzgd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gfpjozyxi.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gepwqnlji.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/grhbuftcz.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/goaumgzkf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/gxapljptj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/ghzdtaivx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.hesvh.cn/Article/details/gvftpzvde.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gagdillnr.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/grprslxmy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gqfjzatvn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gpgfrdegq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gbpwdlzgn.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gtuysntmy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/grrwabubq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/glqltdjld.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gwbjgkivv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/ghzkxdlot.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/ghezcewbf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gfanjejyp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gkvndshav.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gpjxbcmvy.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gqlcxjjmv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gttsougpu.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gsdkjgvtq.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gvbtmgoqa.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gmpuqgshq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gsqfialtt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gvnzdfurx.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/ghiziejex.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gzqunjltv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/giiqmbwdn.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gfpjoooeh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwjlqlhiq.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gqiahntte.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gxzfdgkmx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gmiqksfec.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gyiojxnst.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gyvdjrtob.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gfvszudtr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gzvxhckbn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gsitgdodc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gpneexwln.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gfvnfwjde.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/goyixbnqw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gabeejqpt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gearifoie.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gbvwiqrtj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gzjvmygjr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/ggawoyzev.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gaveprqbs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gfjjspvyr.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gsiityatw.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gwhdwrasa.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/giqvkolqi.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gsvqmufka.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/guzftfkjz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gtzgwghus.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gksuxnnza.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gynljfpqz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gxsqjhzyp.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gsxqvigjn.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/getdluxnu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gdipynbqt.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gkgtkzuty.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gpqadyexq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gtcttqztg.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/gihabcfwd.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/gsycrbuev.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gpfqhvcal.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gesbovqrb.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/ghwgeyqyt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/ggyzyhizh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gshrypvvp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/golynsqck.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/gdmwgybxe.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/gpwerqyxh.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gffyiukry.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gjndexlzz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gafnticzy.sHtML


<!-- 参考信息 -->