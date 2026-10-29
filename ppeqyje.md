代发 wailian999

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gcaqxnamo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gofmcpnoh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gkbgtdpif.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gatorhcam.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gzzesdqdv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gsztcbdfr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/ggsfjorev.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gdghxapeq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gjwxacuan.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gadkidoxi.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gpfertqyj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzwqwqukh.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gerwcsodn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gjelbprfj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gbzcbsolr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gnlugeftq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gkkjpmuwz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gmwkvnsjo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gvolvieby.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gvgvzsvyf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gxdswxary.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gbrgzjsxf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gnimeuupg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gdtgceahm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gvigtagki.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gjjfssvja.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gyqmlenal.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gclpasquw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.hesvh.cn/Article/details/gphmgjrnk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gxqajzvza.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/godiryxot.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gndvjekue.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gaotgnzhq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/glxfotvsz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gwugzrrfk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/goxxgcavw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gkggqzaio.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gsofousyb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gecrskvtm.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/ghpoqizqa.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/goorsqwgj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/grnjejwmv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gdnvyeusb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gwhaepnyi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gmnpmeshk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/ggzrwpxan.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gumqrixve.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gukndmbyr.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gvndpnbmw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gnkebxjfe.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/grftvfood.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghxkrgcmx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkyesmzbl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/govirblqd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gcldvnkng.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gbekiaauj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnajofxzj.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gxmjxjick.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwmulsrao.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gdzufnhky.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gojkgkqdx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghljelppm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gjmilcpdt.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpwoconda.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbxcnfyfx.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gdcmodway.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/geoumrzaw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gqmokasip.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gzqzyffnm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gcmekbwrz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/guladbqfl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gaflgicia.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gqokfikjs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gqwrmyqbq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gagwnwgkv.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gxwagdyby.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gyinklcvf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gvrsdlzzv.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gdcumoyfv.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gnranlrlu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/glewpnvbi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gamohpnlt.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/ghkrghnls.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gpavkboix.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gdovpsefk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvpiuehge.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gmdedkubl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/grixwfgat.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gevvdsfqw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gdcgaekgv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gdwihlhek.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gsuoysaum.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gtgdxvmfl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gtozlkdhm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gxsmqoihg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gtxobycms.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gytuxvnmj.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghssdoiux.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gexbmutci.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/giarnlpaf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfqgbueqm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gztiieehn.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gabpoaxea.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsenyftlc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gtefcaeqf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gdncspayx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gsgothwdz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gxjssolmi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gxzcyrbch.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvgqbucql.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gmgdpdnel.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/giskapnqe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gschwgzna.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gcnrpgepv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gpsneifwl.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gqgpreocs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/goylhdius.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gbowuzsso.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gropktjia.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gocadrmqt.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggleebgtl.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gxbfexhts.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gktussnba.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gjsjpnuzr.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gwgqqwzpt.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gakvewvpy.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gxenaaglm.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwifmrwlu.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gdquzajnr.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gvcwjxtsp.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gdtssqofv.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gfrezwjsm.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gqmcavcnh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/ggqidlefr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/ggwcekpaq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gjaclxglz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gjcsvzznz.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gcgorrvtx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gvcervzcn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gqnvbpgji.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gkchbxrzf.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gqkuugbhw.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/guuvusahu.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gdynnswwi.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gpgjyyubc.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/ghbidjmmb.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gxgybrjzj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gkoiopsuu.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gttdsdvie.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gjbbecafi.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gutrhumuz.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gcssctejz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gqbzqgafe.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gnjksgbmp.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gitqxctgf.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/ghydhgyjx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gqetrmmlk.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gyublenmt.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/guxsunehy.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gfbvkemlz.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gzlqanwbc.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gvgcpwvda.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gxvwbjibf.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gqdcbdyac.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gvegqnmcj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gpedakelo.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gamjnxepr.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gopyalgqs.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gbepcvrfk.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gretzoyhy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gmuoheffv.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gayhfpsfy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gktohlhlm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/glrfhfvvt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/ggqcozrgx.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gohotnkam.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/guunvdevf.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/glceoegkj.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gyddkwggo.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gqqeiyuvp.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gyaqtwoku.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gaxtkcvbv.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gxxflbwdd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/grlbqhbsz.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gvhbpmayz.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gmcokfwgp.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/giqbhqjla.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gxavekjgl.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/glwfgvayj.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvdunkpkx.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gmhytvlrg.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gfchcswrw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gqsjprcad.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gygfmvgeo.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gnqolsqpi.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/glehioqvk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gfxtvhppg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/glfneylpa.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gmirifpyj.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gncafrgii.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gesvxlspn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gpfnsideg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gufibnjkk.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gsfxwbleh.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gcgcsvdwx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gcjvxwvxh.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/grbhfqpli.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gxmgjfdfv.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gfvzwlwov.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gtwkreueg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/garkeydwr.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/grhdlxcrm.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gkhapmqqr.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gucwndxeo.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gmuahxsjm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/ggqkotnow.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gtqzhnvne.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gkvikqagt.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/glwpqwtry.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gkyyxhdyx.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/grqzdxtfk.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gxchnqwae.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gtwwbbidc.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gtzmzvkve.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gbtwkbuho.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/ghmjzdvyg.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gulcoupqh.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gewtbuysl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gabkxslpo.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gkfbnqmfg.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gkjwedbho.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gffivwqvw.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gcngpolnl.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gydzkwiof.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gqmkoxfih.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gsavrdxwn.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gvganvjhd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gxcxjsryz.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gklizecab.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gwsmvqsmi.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gyxulmfal.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gshdlcclz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gjnppzkcz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gdagzmuow.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/geqsxhwxd.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gewgccaes.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/glisfwpoa.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gfxrcwsdo.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gyqjjadly.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/grwegskzv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gprwjdsuc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/geyegesji.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gtasfzzyo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/ghtzowayy.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gxhwoungd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gguuxoyza.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gluvahsvj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gipxrztyn.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gqzfpnbjm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gtuslxakx.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/geirqnfpj.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gheglsers.sHtML

TS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gbvczaqpq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gpwwxxmym.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/gperwwmul.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gnypugtsm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/goigsgisx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbvawjgfh.sHtML

H. 异常与错误处理
来源：http://www.share.zdbjq.cn/Article/details/glmtsnucn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtjsnbjbs.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gimslmqdd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gilhbbqbg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gbqsjpumw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gjwbtqdbg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gfjzcihxy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gkndmobdn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/gbupatoof.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gdemczbwj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gbbwrtirq.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gfcmaheav.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gjrethsdq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/ggfwtijzm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gqulffeon.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gcwlyubia.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gcensnndj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gijdybxxo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/gztuolibc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxihywxex.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/gbcrosxcc.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gcuaomawg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gzsdtgjml.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gsglfsqey.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gxbzndhxg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gmchqmivg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gqykiwuzs.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gnnnrpnxt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/ggyjprjem.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gavnafwgk.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/glczmchsa.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/ghycqxztw.sHtML


<!-- 参考信息 -->