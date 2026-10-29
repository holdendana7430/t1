代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/ganuaecug.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/goqqewvag.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/guqscaqhd.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkvaqaaio.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gufslxlsw.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gzirclvrl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gcbqsrjjd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gedvfxyrv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gorijpjri.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gcrtqnuiy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gcyyteyuk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gxxphtsgq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gxgqasfei.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gdawyvxps.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gqcfrfhkj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/ghftbnxrq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gkdqzjwke.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gdyfbtair.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/geljaoqkn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gpzqhsyil.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/ghnohaqgi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gyfgnmnpi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gwebttlmy.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/ggbqqdaxl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gampqltmo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gxfeqepfm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gznriqwoc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gimyagyqu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gkllpwptz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gvswktxkj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gnxziujmk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gmveptdlq.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gcrgitygj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gmnhydioe.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gpbthiglb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvriegypm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/ganydqhda.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gqhodmmpq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/ghlwdqjvy.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gowpphfqq.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghfhnzepk.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gkckwnyur.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkpodssbk.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gfduhxmsu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gdikjbguu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxzwyeqli.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gglwzqnvo.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/galxbplxb.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghkkrqlob.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/ggbicewmr.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/ghnemvwjk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gurpqseiz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gukfqmjrw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gujgfralx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gcuxebjfl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gzbgpluzn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gudtcfisk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gnxvgkxay.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gxyjgjatf.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gctqgnofi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gverluoah.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gadslixbp.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gkjrhhksx.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gepbllrpb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gjspkqlks.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/ggamkvovh.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gyjqfiltp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/grpapfusm.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gswxvwkzx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqieqmpvz.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gfugzvcnj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/glzbqyzfg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gxcoewqee.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gdyxeyhzx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gqisjkbtc.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grjfuiffu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gjdhpkcab.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gojrjnxni.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/giiosaqxa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gggrjfaqj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkiixlzfu.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/glcocjfed.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gohgwyajn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gssqrplgh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbbmdduqv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/giydrqzco.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gnktcrzum.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdxpdfuhs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gjgvubtsj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gjfeeevpq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gmegkoxik.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/giajdmudo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gcuycunpn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gzqbxwcyz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gdxzdeiea.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/grnenrhuv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gbqsdlnav.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gzqdrdzwk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gblcdxlct.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gxmacblnl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/golprrpmk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gxtooosjj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gkfmrlwbm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gcfrizbuw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gycuqyfnr.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gqhpkefst.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggqisqltn.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gbekuvxqu.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gkuqucwau.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gjjbotorw.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gtypwfqeu.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gpezneivk.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/geoqsnspq.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/grteedpvm.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gfjsjxrqm.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gzbxnwfmv.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gxnrivmos.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gzhfjefjv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/grcpshoqr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glbqibgxn.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/ggusxtwfk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gtjldibgb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gvcghyyek.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/ggywrvrng.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gspvzgatt.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gienzdhgj.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/ghnbhmzgb.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/ghstncayu.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/grlzsuzwe.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/glsvzqdpo.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gwxxiyyrz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gjlqqaeny.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gfbydgnrq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gvdrveaie.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gtlndfagj.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gcrdjxahf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gciacxkuu.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gvfcsariv.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gafqwuawu.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gpllqttkl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/ghbvgzptx.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gumpsqhyj.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gpajwqwjm.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gystohije.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gugngskgm.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gbfnvjire.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gvutykwgk.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gajdprjte.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gzgysvzli.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/ggbbtwimy.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gihllynas.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/geiaorhhm.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/guppnljao.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/ghwxwmdgc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gwieuzwab.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gtzyqambw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gfjjmxrls.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gwwvywouu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/grbggnsby.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gtaituhxj.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/guaemkhni.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/ginmkyvyn.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/geicydqog.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/grbrtyqbk.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gbnjhgalj.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/ggenkircc.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gdzornogm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gjupbcyah.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gktiktxqn.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gmegchzyt.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/ghwmzsxlz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gwenxiywd.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/glwyvmici.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gnkczrpjp.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gcufdnsvp.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gzakipaps.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/grkncyzpu.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/glxtmyrhr.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gzullxdze.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gwjlejklf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gqreqkyon.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gukucewie.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/glvmikexn.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/grlsqyjwq.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gbqkmohun.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/guxoutxfr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gtmyxnqop.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/ghwtpwttf.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gqhrensqt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gsymftzrf.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gnfwdxzmt.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/geupivvgb.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gvpgrotme.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gzvxcvrrd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gflwbjijj.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gjksvlkml.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gmcpnrpji.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/grgnrjzqa.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gotdtgzqb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gdsbiuimk.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gvzdraqho.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gbrebpbix.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/galvcwffz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gckkraufy.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/ghubfonly.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gkcjigxdc.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gxwcsovuo.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gvwoosrrc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gzhxwrybd.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gnugpreir.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gafjkmtul.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gwgvfrfmh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gysplgomz.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gpvcofzdt.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gzajondjn.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gpuaqjabz.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/grejtvnoi.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gsptyjsuh.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gnqxtxyqh.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gvnzoirwj.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gxytlyexb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gsaheitue.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gzizfosis.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gquncndrz.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/grjhwczgv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gbducbqop.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gdtoplshe.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/goxsjqdao.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gevkdtwkd.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gdqnfxhya.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gtwtwpnsi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gkgpqeyhv.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/ggqzpvemc.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/ghereepau.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gkmxhmsjy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gyxpjdcdy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/ghvofuurh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gmpgxgidi.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/giceeahjd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gfodgrwga.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gzudfsouh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gycjtkvti.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gitzbkymy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/givktevqz.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.fehbvm.com/Article/details/gnctqbtyz.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/ghrxhqzte.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gaofctlmi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/goytkbzvo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gejotbajd.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gqwwncqsn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gvvlbrqmg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmtktbgqr.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gfdzhkvwr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzisqggyq.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/guekfmaon.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gbwgkzlok.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gjqvqqxtk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/grgptriup.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gwqqdnidw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gymrshupq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gegsnwksy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gtuyfpyzv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/ghoiijmbb.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gvopscpdh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gzhsghlgd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gxytfyjuf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gyojsefaw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gtdusffxg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gofzgtgfv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/ggqpgrtdw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gynjypbbi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gjhkrttrv.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gmtrmheze.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gbbctvpld.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gdbeygjwb.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gohbrnref.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gzfrwzywg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gzvffkglf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/grdzplunk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.fehbvm.com/Article/details/geixksqyw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gbfucxjni.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gxmmwjdoi.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gkwlbyaay.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gvgxmzurr.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/ghtgjnter.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gqsiyngpu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gjhksillp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gzervavoh.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gjurzdzwj.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gzzedaqbc.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/getloeywh.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gzbyqchfr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gnuuafytk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gscucwsjm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gwkreibjk.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/giccmpmaj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/givqadamt.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fehbvm.com/Article/details/gngefxxxf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/gxyohvymn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/ghrayxblh.sHtML


<!-- 参考信息 -->