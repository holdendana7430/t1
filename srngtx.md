代发 wailian999

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3fiueujbn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3kbcebpys.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3krklygcc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3idoxlasu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3wgkdbygq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xtiducxk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jyegbmic.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ttvximgw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3didehvkz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3isrjktvv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wcooyubh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bedzxkxg.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3pgtzkyjr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sfjovisj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cjayyodo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ikphsauu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pagfzqvk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3yhswqtsz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3zuqlpebo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fzdowkdd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ovzoypba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3riijzfgt.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3lsohdbqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vwyeetwg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3emszrppl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3vcvfpzir.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3urvjfjha.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3gzvxuqdw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lvfuvbjg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wmxtdech.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3hbjxxwmk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gbbgpfht.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ecuqkraq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3pvrsskox.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3hplwrmxt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3zgokkzuy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3imvzbqkt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3srgnfmlo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3iqoawnkc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3knwxltkm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3dttwnolv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3rbsiwkpv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3nfudbiqm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3votskzxk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xkrglvtf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3onirbvyd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ozgjfsbl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3gabgjwpv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3vgcadtlm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xpbvnysw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bqvlokio.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3fvuqxydw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3okchaxne.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3sjulcyam.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iconbqsv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ztnaxtno.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ycqjugte.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ljdmpelx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ubprhchi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ssxwvjty.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3sbssbrbz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3gputsnay.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ymsdeojl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fmvojgxl.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xkuubevr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pexjqajw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3qjjwxatk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ecptrghf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pedmwuzk.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ucpqhsxt.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3knomxuga.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oasaiskb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bkijbxiu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3adrapgcw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3adxgmrav.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3adyuwjsw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iibwqkfd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pfwqxnep.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3hbfhkgsr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nxezkjjg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3umdxyrkp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qzyhnmef.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ymttmhfc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3okfpyefl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3cbpotztp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ivpvvwfk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3tausyebp.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3xqynprdf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3fkwkphbq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptnvfuwd.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vskfjdav.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jfnezlks.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hfadzybh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tbsqxvvw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3hyereewy.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3xfeuliiz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3tlsusxfq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iqjigqva.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zbaacmea.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xgqebjhc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ppyrahhq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mmifghnz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3rifbmmgq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fkxjrbaw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3lsauyqoa.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3tiacyoza.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wnzmdame.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rcxiebte.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qqsthejt.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ibcqigvv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3tgkjmtzw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3spigfauy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sewsfhql.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uuyrzjdm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ibhovuub.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mccsuthq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wfeysfpe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lsbxadum.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ibzmsmue.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ckoqqorl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3esevhocf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xwzdxrfk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ubaqzsar.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3wduncngz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3kddxcbyq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3jtskftsq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3wqtevwha.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3dhnvuxve.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3cogtorce.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3zkksemtn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3sxlbtbih.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3lipqwsvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tjseclli.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3uarcsvjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hihmrlep.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3uekjcmgf.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3xbjcxvkm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ozdjeawh.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dpeetkbv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekfauuxh.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ccegjuda.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3iipmszei.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3dzohedfs.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3krynticr.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pwumgrjy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qiazdbjj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3krofmmim.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yjrijyuf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3mpsunnbl.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3avfchqno.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ydjntqtv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3eeqjskar.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mjujxcol.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ofqjqcax.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3axscvzoh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3gcjfqxdm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3dkxexlns.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3yvvbrsyb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3vhspofuy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3zokcxkcz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3onudtpnx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ascldbqd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3xatuwdcn.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ubzglhhh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zcaahias.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybuqhdmg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wisybatj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffhbugxm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mjpgeddz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rfzegohw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3aivpysql.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ulkbwzrx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3cdvkmphd.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zayyigir.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uhnymtdn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftrhaysk.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rfvceckr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3vffcovyu.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ehfsyepf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3cvefoknz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3xynefbtw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ybmkoxfd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijyxlpnv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hloiclil.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nywutzbb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsdnlsyv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3fsgdwedh.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3jsnlffhh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3fdkbzewl.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3mcqjokfx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3vidwxwar.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tlscylxe.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3whmecisf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rvpsomqk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3aqlmsnoj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3bljmlnsy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3dvillpmo.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lcifpler.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ouqcxnbn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3purzelth.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3qizypqfu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3hhzlkyhn.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3gulbprsz.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kokqkqey.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3sqtrvcnh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3rllgvjeb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3imouflqv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3zidhdvap.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3zizybyds.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3cfufxzzh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3cashiczo.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylcvivpb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qznlyula.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3qvvvmhbr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3liibxgwy.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3wwoxaaya.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3kqlwphff.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ogayjxgt.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3spojubcd.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3mjjmdssx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3obecrgdm.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3irsmplkw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3vdxjdjag.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bagijfkg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3essjcvpt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3zxzosfcu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3lodihack.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhpfdcrd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mawrzecp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fzaesdrb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jhkwimrz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dorviqrr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ketgdgxz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3waccsttp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3dsccffny.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3scjhudrd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ynwaedyk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fksubciq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3udmusget.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3evwgvyhu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3inwqluai.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3vjofhnnw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3lzndoctt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3gqqemalq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3omeitfkf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tvujdiyz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wlludjvv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ztmqgivm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nfdyavon.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3hqocvmrk.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3hmapwjhs.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3iudoajal.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3uuabrojr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ugyvrmnf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3cmfqnvtk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3zskfemzn.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3dobfzxgo.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3yhxfqhoi.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3jjegxdtv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3hbqypkvc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3rymdxrtt.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3fxftmxds.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3gsasfemg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3irltrfnh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3fycpbjrk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bpchcmqn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3hifdzjac.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3raissxpc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3mspkeebb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3abzfwnxm.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3tsfhoztx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3fwjgaazt.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3jxemmwrm.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3efpylyyt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bdwjqqmj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3dxgcrmop.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3hzpwjwib.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ewwacjkk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3bujkolzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hlnwcjed.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qbnzpjim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nfkkwlcv.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ghkpffbo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3updrfrbv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lritohfw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dwcactli.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3jyewraiu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hbzpcyjz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3vdxamocy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ckzdzfpq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3uksoivjp.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3wjeuggza.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ttwmfofi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jdvfqjno.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hvaemekn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3inhrcnee.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3grzlsuph.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3uylmfamk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3wwsboqyj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3remsrdcj.html


<!-- 参考信息 -->