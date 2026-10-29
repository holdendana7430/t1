代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gdkljmwaf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gaqsjwhya.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gomfmzyam.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gdphtfgta.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/ggmceoioo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/goinnxbak.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gxcebhaoi.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gtiretthh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gkterrgth.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gddkkrpae.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gbgcfzxxc.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ghmmnuoma.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/glnzljaxl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gqsuftpbi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ginekojnf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gaqhqqywu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/glpzwwbha.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/golecgeiw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gcxqkqvih.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/goclixohy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gljoaosff.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/ghauxbujl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gmernrhvm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gqwajjzyy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gppwealkw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/guxyhoqzj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gpckjjkza.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gpzdggxuf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gqfgypmmx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gmlnxfdbf.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gziieolvt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gsucuuacb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gqulwycdh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gymkeffly.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gwoeklukp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/guujznske.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/grrojohdh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gpwpovnji.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gisfpjbtc.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gmnihqvfg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/ghvmzlxau.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/grswkpwgd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gvowxsauc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gwcgprvqi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gcquiwall.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gqkarujmv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gfexiegiv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gqpanfqcr.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gtipctzlc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gaczduwji.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gtznazjbq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbexedeod.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/germmyclc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gmrgtghwi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gydubpqeo.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzitvtazx.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gocjrnklf.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/goxalpoml.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gthgyixtf.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gdajljlre.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gusxzigav.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gckilrsnf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/ggejbzqom.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfmceivrd.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtmsotrqr.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gndetopkj.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gvafpvxhv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gsencehih.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gfgrknqnv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/goigfdyjv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/ghdlfluzi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/glrnisdbm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gbtrubaxa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gkgdnucik.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gcmpbfeyl.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gipjrbihr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gkptjrpyh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gcaiastin.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/glxbpcezw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gqwhesxhu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gywwgkirf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/grunbnurv.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gbpdnnund.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gtsskpjwe.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/ghyjvnxuz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/guomgsenx.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gvzrjxlbz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gdkyjfajf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/ghxzfrqse.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/ggugjtofw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gyayktact.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glwficaii.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gsrxlhepi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gwtohuike.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gmuzkejgv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqxesmxyj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvnjdkont.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gzywlwhuw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/ghmqykepk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grylbckgj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/glophesxu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjnkfpxcq.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gdyoxoorw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdwmgondi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gjdrvnjcg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gvowhekkl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gnyjomzmy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gkrtjyhwz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gndniyxgc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gszvnfsym.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gvrieuaoy.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/glugdfuho.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gceqsynzm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.hesvh.cn/Article/details/ghryabvaa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gfmmowkjh.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/ghnmzottj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gnuxyrmwh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/ggkxvhspq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gssnrxser.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gjbectwgd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfxdxpwox.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gymtbhgzj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzguyjemw.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gpvnzhwce.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/geyqqxiaa.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/ghedboqdr.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gvtararfh.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gwnfbgcgq.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gypboqcmh.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/grmccswyp.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gfqcvxyua.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gzmcvmjdn.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gmwxfwfcq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gqiiklhse.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gyqqsqiye.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/ghqlghlze.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gxgykqjtu.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/guhctoujq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gtzrhpryv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/ggushnnvy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gqqnpbkyv.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gjdjahubj.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/guotlseqp.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gidnnsqrd.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gwudjufkz.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gsjoquvzz.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gqbxwrcea.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gdqlqgqte.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gdgozrawf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gaoudzfnl.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/grfdqssor.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gqxqwplii.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gmsnvqbbi.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gblarqysw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gawqxnvll.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/glxhpnhio.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gqmorxaof.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/glcgkqzsq.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gdjcwjayg.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/ginxgjhyw.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/groraahsv.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gggpxjifz.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gwqkibzay.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/ggdcqbrhw.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/glvkvjuzo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gcwiusvdc.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gdufrfiuz.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gtaqbfwjm.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/ggqtdvpew.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/grhcyeplr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gokdgojtt.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gnxgjwume.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gsjqmcpfy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gvknvqsja.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gbhytcyri.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gqqtcrfgt.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gavepizhr.sHtML

[G07] 调用父类方法
来源：http://www.share.fehbvm.com/Article/details/ggaamfacv.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/greoesrra.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gncohfzam.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gdcjkoefp.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gcpciqtbh.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/grcvkuzky.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/ggkknzkza.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/govjipfdu.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gqnizjzbk.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gmnualkza.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gfyyqenqz.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gmzfeiigl.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gxpukqjec.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gorgapowd.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gfidhtuov.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gedqohoam.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gllpdvvng.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gsmovcvvb.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gffsimwux.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gmmmgbjjk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/guvnqizdm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gngwemktn.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gwjolltmg.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/grtlqkgom.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gotwhxonc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gspvlvrvh.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghnfvtelr.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gaxuwhdyv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gpfkdbkzt.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gcbtcitwe.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gkermzyow.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gistcwllx.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gqceeypzk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gztqyggvd.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gjeitzpbx.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/guwdbljjp.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gaknybbcd.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gaqvrkczj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gulkusswh.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gckfydojr.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gwooffhev.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gjdryylmu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gmtndnnwf.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gnmqitttz.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gbovovhcw.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/grkejfvlj.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gzceklekn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/geaisoxkx.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gptxbfnir.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gliftrtex.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/ggbjymqlr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gvqhgnykd.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gbhbchhoz.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/gwebojsnf.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gnmlzmsls.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/ghnmormhy.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gwqgjlkic.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gilopopfk.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gjutysnqz.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gjmirfyga.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gowxnahfu.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/gqbtjzpvr.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gwozimdtu.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gzeeersaf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gissmkvpk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gnlausxyr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gfhunqblf.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/gvbaszlfd.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/glzgelmcd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/ghehghqde.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gxbwqnidu.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/goonaytvq.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gbdslndok.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gxceatfoz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gvhtkjcav.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gagnuaaip.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gfhgmvcgm.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gbqhidmkp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gofanpyqw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/glmnejtzz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gdnshzvpp.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gkhapeaby.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/gtarwqtiw.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gzpdsggjz.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gndarbstt.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gxxzldoen.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gbvizunpw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/ggblclopr.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/goxqzgnoj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gbcebgtbo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjdsvntks.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gnhxahqkh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtqullsqb.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/ggrlcpjjf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gdydevcce.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gpvzbsjne.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gasjmljdo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/ghnzlhfiv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/grlgltmca.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/ggnnmcgfb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gxwhgmmbm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gvecbhxdl.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gcnuskzut.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gqeobtcnf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/ghmvivwpj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/ggvnsztop.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gjewchgwa.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gaqodkdoi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/gcapaejki.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gjkfnzsno.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gypidgvpu.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gcxkehokm.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/glwfngpfn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/ghnbwuutz.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gkeaytzlo.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gttbdcglb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gsefvdrih.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gifwflfsw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gtnpligcy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gwdzuqgrg.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gnfnrshzl.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gesbvyubu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/guqcpvwew.sHtML


<!-- 参考信息 -->