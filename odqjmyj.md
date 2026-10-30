代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gpeluvarr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/ggvinfmzy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gexjiwdge.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gavvlneoo.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gxghbelfa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gshxiylnk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gsgylrlbq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gziwekedb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gehdbkbvo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gxgzlmczr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gpgkafgvc.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gvfgahlqu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gvngxmmuo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcxsioxbj.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gbkgbppbn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkjidkubz.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gykvomsls.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/grxpubeop.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gwaklpaps.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/geezfgtsy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gbcqhgqfh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gqhrlusar.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gctcqdpab.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqsqlmshb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gllcymlbn.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gkwwbqxwl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gdrrtwrdv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/glmauogfx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/glgkyfdic.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gpgzqshvs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gzdmluwul.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gnjdoheqq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gvrgikkva.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gxrmorfiu.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gvxbcxgkh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/ghxkankzo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gpeypfztg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/grkluavbb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/guoobvvbq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gxpynwyyo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gubwnocow.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gpqomjuvz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/goafnqudj.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gtywebkmk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gabafyoky.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gtaekifzk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gygyfnojq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gfescfoks.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gaylfsdlf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gbamddqlh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gwtvhrdql.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/guaodtikx.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gafbxavtp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gumhwzira.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gscsnmyll.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gpndsuqzz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gexwxzjuj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/grlyamylj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gusnxafen.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ggqjowjoj.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghvpwqjvi.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gtgggaqcg.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfkwfaaoe.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gpllwbuje.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmduuqsec.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtlnkiyxt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gpelzautq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxubhegjr.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gybvnhpdm.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gruvkxiqv.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gxjnoebzu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gkrhmespb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/guaatvtgj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gtgixwevg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gidwtskyx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gwcqlopap.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gcqrjcvqi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gnynheoav.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gwxbdwakn.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gelahdper.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/guxaausmi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/ggroxyzuo.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gpqprnvic.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gvwrpcylc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gdubucheb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gmovagtvc.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gcnbtuzqk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gwxchuwie.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gqqaobqwg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gorajrfye.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/ghwzfaghv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gyqcpxktc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gzczbemvt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/guehlrxbp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gpsxkyjml.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkfpitpwc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/ginusxqpe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gbttrxokg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzkkzoybt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gymymkphg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gyqxewokd.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gferdhsrh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gpgiwqtqy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghioogdrg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gwjjqpdsi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gthtkjcti.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gvlyqdvzp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gispjugql.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gmqnlsfmd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gsgljwwdh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcbyjfvst.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gyrwwkgji.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gtdaibxpj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gxzoybzua.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/grltfpoeo.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gfkavccvj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gqxsyvwrl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gklevnmzg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gppziwamo.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gcowicafc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gyoaayrzb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gssbbjzob.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/geoebhcvl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gzanmxutg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggnxgjbhj.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gdiubcral.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdaksanvm.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/grdtyjfxy.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/geteobptg.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/gtjxbkljs.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gfhmwrsbr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/guyzgzboq.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gjvcafcip.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gyiwbpioi.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gdopnipbc.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/ghckyhjjh.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gnvwzejgm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gcoqwxrbf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gytdjehzz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gcikxycfj.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gkjmnazvp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtsktubnd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gylvccdsk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gazibuldh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gactvovvi.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gipdhpaqd.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gbzcjmkyw.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gshnwrbms.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gezgxwyra.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gmjsuxfui.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gjbajbuyn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gavjddaow.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/geyzoguxc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gehrkoemd.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gdufsxoat.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gbgffauxr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/ghbptqvrp.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gnzkdcmfg.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gdzcqfewy.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gwiozdpdj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gfarszzum.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gbfowodtw.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gjcrsltpb.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gpbaibmbs.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gehhrmjxz.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gguptkrsl.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gjndsnphm.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gspooqorv.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gwacjqfko.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gejirvcys.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.hesvh.cn/Article/details/gmqygvusl.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gojsnsljq.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/geolikjqz.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gheeckeae.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gscwthqut.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gopxviuia.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gisbzbbrm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/giagvrvzs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gohvmgkim.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gwaqztvah.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/greelepju.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gvrnkxunp.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gncocbiel.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gjxzcwsrz.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gyoswybnl.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gkxffhfwb.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gnbdtuqal.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gviuncvrh.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gzaxitibu.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gtfbpimzp.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gqrvjzktf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gsweyxgvr.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gbkdkybjn.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/goftgfupk.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gdwperxgj.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gsyehhxnp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gqvsaekdg.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gcmpfvyjj.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gsgtafqex.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/geyzltnnp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gyijrnivw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/grsuzrqrg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gwcvjfocy.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gvpcsbvpj.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gatjvbsjv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gkiukxkyg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gnivutrxn.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gbdehoftt.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/guhbrefuj.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gctrkwvqx.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gimahsjrt.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gpcalistl.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/glwnpibjl.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gvijoarhd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gstcvurdp.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gmixtprtv.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gsoczgsuz.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gthwtrzcy.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gisuldrpu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gorpavktm.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gglwegxrc.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtmmzkxas.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gxmwqgxuk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gosgauroa.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gmomzwxsi.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/grpkbyaku.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gnjumsglk.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gajdesgem.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gletzcnga.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gczfobeev.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gypbchiib.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gveanlndj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gaswffagq.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gnzpkjmuj.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gzsnrrtka.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gpqnxpxzh.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gxmpbmhrd.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gypfxqejl.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gxlmuipft.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gelirkcki.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gfazlnjep.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gwptohcgs.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gnvwavhxh.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/glqjzxnwq.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gdirmcrdh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/ggubgbnvt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gwljaxjuy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/goesrcozu.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gaqkfoxxq.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gjynpghuv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/guihicpsk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/ghkjydoyk.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gbewqtmcm.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gfgrpyecx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/griyrkkif.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gibnmrlgb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gcjbwiipk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/giocfmkib.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gaxobhnfi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/ghvujgzxq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gzhjqvzpw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gbmpbavrl.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/goxlhpwip.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/glhnulfot.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gqvkudfzz.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/grzxqwyvl.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gafpsysac.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gtaluknez.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gyeaotbvb.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gbsdeufip.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gpwgzhgbw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghdjtbwol.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/guqyzjjjm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gayrqfzii.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gnorjsfjp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gxsbjrwly.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gtiolrwez.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gjvxuthxp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gzuyayfyx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gimjankga.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.zdbjq.cn/Article/details/gnoheenlc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.zdbjq.cn/Article/details/gloxhzhyw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gteeypbzt.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gfksxgumd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/gjbchxkid.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/giahfdtjj.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gpjgqydxo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gqwdhyfhw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gqpzxmibz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gijiudhto.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gjazndjzg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gnwhlppif.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/ghmduyuat.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gkyimwfof.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gasnfqdoo.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gerjpbixb.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gvmuctdgd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gplarcemr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/gnzpverlu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/ghwctfzus.sHtML


<!-- 参考信息 -->