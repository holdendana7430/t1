代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gqiplqevm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gpgabwjrj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gjogbogpt.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grroevjeh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gjwosqwze.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/ghepkcpfj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gdswztvky.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gyjdxqudv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gecrnudsp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gedtstywo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gmqkplesn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/geamghmwz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gazsjgqxv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gxpcpbjby.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/glazxoksu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gbbfdkqkh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/grroudmbc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gdmypbpaa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gcyzpfvoc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/glpzaigid.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gpnxeaphz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/grcpkoaze.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gscscjmhe.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gspejvcnd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gjbsxhwwl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gancdpbkn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/goqyrckwl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gxtszlzlt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gmfntdiex.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gdpahtwim.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gufviesfd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/giasstdwi.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gokwiburi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/grktlkptb.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gjcotmsdi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gskiqfuqc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzxdnzyrw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gfhserplh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/goiepbsqj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzeajnrea.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqsyfkwph.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gdpkwejos.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gefwkvtec.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gjsuzakvq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gviodfbex.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtiuwobum.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gzhdpsdno.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/ggnopwrmj.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtpfnzvaq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gjenvxgso.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gwvkipnpm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gssysjuqf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gcxuavzao.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gbwyhzvnp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gebgrkkle.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gxsiijhvg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gzbcndsoa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gerxiausm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/googsdzzg.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gasavzcxb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gcepthhsn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gkkpggcuj.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gzvtujebw.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/goegcyglx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/galvopxst.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gslakiekl.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gtjxlombq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gywhpwsrv.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/ggwduiips.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/glnofzbgk.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gcflogxmw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gbqtxkrnn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gugfqeodj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gjvnkkkxx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gjkhuaxhl.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtlootuij.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/glkhlnvxy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/ggyzxuhgp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gftqueduf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gsrcilfss.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gliacrfbf.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdnrtfqst.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gxohwpqgl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gmieyhtli.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gznelzfel.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnbyarbya.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gtxyvipaa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcbwwqxny.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gswjvxdru.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gmamqnxef.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/goizuznzg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gdecdvjal.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/golkwdzud.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gjxankmno.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gdjlpfkpp.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gqrshtzcx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gjnontbtj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gdgrosprv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gljanyzww.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gabylnchb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gpxgnnjnp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gvybppbiw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gdtjytbxa.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gbyjixtxe.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gewghnobb.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gqbpzhrbz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gozlwsxnm.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gcmoxnoym.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gdeebwovy.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/ghkixjztm.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gjozdkunp.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/ghifpnuqj.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gaabnpwdm.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gzqdrjhwl.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gwnqpzrqj.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gnktekuei.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/goxabybdv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gshxbzeun.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gpxtzclfk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/giuaqsmph.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gieekthjs.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gdftzesqh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gsmchzkss.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gbmzutxuu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gpdfwgazo.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gmmwigqpw.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gbtakmzvm.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/glgqyzyrd.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gbnmznjkp.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gvkfqgjpm.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gmjdvmiig.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/geefldplh.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/geupurflg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gezgpgpho.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/goglxtlsm.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gyazycjqo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gcledsckp.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gczweuwfs.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gkbjzdgnd.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/groeuykgx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/ggjceuvxg.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gyqpkoquy.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/glfdaldvo.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/ghxxejhif.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/glxnosfhv.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gmbgcudoz.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/guvbmksyf.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/grloarjsg.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gsavvcfdd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gnbxztazj.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gciwejtsx.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gjucuqpox.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/glwefekfa.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gcxitcktt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gsiaqbypp.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/getaocbpe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gfosycavr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gjcnmfdrz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gqbdxawqh.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/geoboerzl.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gjxrbxczz.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/goamrgtur.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gkdqkohnt.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gdltbdwso.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/grgbgjajl.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gnijwahqe.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gacxhdbsj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gmxsiunka.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gtiiuiixe.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gklprsajc.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/geofehmdt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gjtjanxdn.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gzwalpdod.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gefbkeooi.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gfbtqawxs.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/glodznpkr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gttedlntv.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gvlsgdarw.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gljfzdiqj.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gtonpgpar.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gkwotzwfr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gdzozwohb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gfexsjykk.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gfbxyfwfk.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gwxyfkpsj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gkbkvkhar.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gklhzsjkd.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gfcudscdc.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gyfosacmq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gxtfiitog.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/ghejrwqgt.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gcvrvuzqs.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gkzzuqwzb.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gmpdtujfa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/ghsjtaqgt.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gbrhjcsfp.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gnujdognj.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gcgatdnsd.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/grvvtasmp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gzzcuakhd.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/ggckujsam.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gsjhddcfd.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/grawffvmv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gjnvguuzq.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gifrbfoeh.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gbkawtcjy.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/glsdvzgpw.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gcthrzatt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gxuykresz.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gpunnujmw.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/glnvankro.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/ghzbaooww.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gvcluyxvt.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/glfqgtwfd.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gackiflmf.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gjufuyxqs.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gqbxvxpxh.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gdretdzmb.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gjonipgoz.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gpchjxmjw.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gwzfdqudj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gpthsdxfs.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/glmvtltvt.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/glgmudnmb.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gjtywbdqz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gidjsgvef.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gihxcsdrj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gmprniitm.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gepjrqken.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gttcbinpx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gtnhmtfpl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gaslglfwx.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gknknqxsu.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gwofelaaa.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gcidkpzid.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gvuevnpve.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gusxaxgoq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gxmownelr.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gvhhuymoo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/ginsnxobi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gqeshjnyr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/grofumjdr.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gubnlbast.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gzeoopagj.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gdyzsfcsr.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/ghrkyuvfy.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gaewbzbpj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/ghsrsmfiw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gggbezhkn.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gywsaegmt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gspthqcib.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/geqbntaky.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gdeeokrfp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtrtikdox.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gmafyeelp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gpxdqpmig.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gpbexbxor.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gykphbutt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gskcpokkk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gajuecshg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/gfetycqce.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gpcpnhdow.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/ggmeiqhej.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gelemgrxz.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/gyzkbbxlk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/ggwxrufdi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gingzxinj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gzsoxkbxb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gyyckmghe.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gynrodrpe.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gxforvkjk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gkwruxewk.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/glquznhid.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/ggazquqly.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/ggogefjcb.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gngrwoxwj.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gvvohyyfo.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gyrwfzfts.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/gykohtlio.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gnlxhglht.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gvcvwnllv.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gqavlwxkv.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/goleuqnla.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/gdtqmnhic.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gpzuaptce.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjqzmiiuh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/grrvwclrd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/ggutonagd.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gvkpqrdlm.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcxvfmxjj.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gahpfalck.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gnyootskd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gjjhqrrvw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gdhfuppqs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gxrjyfwdr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/glskypolu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.hesvh.cn/Article/details/gztapiyyk.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/gtzbtkvcx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gpfrrmrva.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gdtrjckfw.sHtML


<!-- 参考信息 -->