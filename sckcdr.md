代发 wailian999

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2nuyhycom.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ewqxfoff.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ogmxnigl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2sjiooehh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2donaytxd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2msjyvzbx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hehtexnt.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ggfyykul.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dcbfyqfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sxdmuohd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2obztyimy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dreeghhx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ddplxsbt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2mwfuuqjg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yuazsbyu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2aczbylcs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ogrszirr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uklriwnr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2meyaolqo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mqesqyjr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vlbshput.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2kyewmmlh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ieuspgdw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lctvolid.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qyywljnk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wqxsezee.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2auqhhdwf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2vuriovyy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2tpansnbo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2gmpyokvj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2hopsjtqi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2smpuipdt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2eexmycqz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pwuedzcj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zozvzcsg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tfdqqjwd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2niddygqj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ouojbbxn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2auerihuh.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2axromrul.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dfokbfvl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2fmmvbbee.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zgxdipsk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ecsljqnl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2nycsbjck.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qxikmiym.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2iplypdiz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2pkngvetm.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2gffcwvgr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ibracgaf.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tfapubco.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gzzuqecq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dzugunpf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2daikbdxc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2fqarabso.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2scumoibf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2owtjiigi.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2zjkhlmxc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2humxanps.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gplmmbbq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vxtagfqp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ncjveciz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qipjidji.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hhbbeuxw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2olvvgcle.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wjqvzajg.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2zkxgenlg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uxfcatht.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ackftvtp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hbsnztai.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rfrqtzgv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2xcjurssg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2jhripmsf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2vklgyhmm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2xcplitrl.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2irwykczs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2kotfynda.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhwzkyrc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2homikqko.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wfyzxalv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hplkzbtk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rqfrydgt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2esbaubng.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tkhzslhh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2jlljscan.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mkdqqzvx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mbawzviz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rawqzzzv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vkwmljxj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jmapzmfl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2kelsbedx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oldvhlcx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2soflqman.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2cmiqfoar.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kklizbkb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ghqzfwbg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xuwlxbha.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ejcitdbh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2biwachzl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eexhxbci.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ytrytabt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hsjdgscb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2xnqqrgtu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rydepgcd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2podedjov.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hyynfxkb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uswhymij.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yknzgjcn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2kqnccgtf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2niowaifm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2vtycgiky.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2mkmwbxqw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ztptkptz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2okuqbjwx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2kyekcwif.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2smypbqfy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2xshokapw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2webncnxu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2tukewdot.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2vnaohlmm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aezosciq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2kqgsigqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ggacsqfe.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2rcsdyqzx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2gscyjuvz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2glxvzamw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vcwjblql.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2xekxwhrp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ctzbkmfg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2tgufmyel.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2qunsayoo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gdiuqbbz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2iqerwwdh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ttohkxir.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpvvecjv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qzjtywqw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kpxfqgxc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2djnqsgbn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2xdjxfmta.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2kctyxwap.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbpsqnkf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2aldamaio.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rtekimui.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2uyneujig.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dwzqplbx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bdkjrwob.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2cendccdm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2cfhsbabd.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2koyvyrjx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2nnsnaqat.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2bdurkewt.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2bqsymzfp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2udfuvltn.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2auykvihf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2odxjeaxc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qitjuplt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mlgpcomn.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bsumunav.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2uhxhhniv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2xylrfqih.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2emitwoen.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jjruihwv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kxstiezg.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtazysvd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nfxdzfln.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2bkxidiyx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2btroayjp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2owgqobhf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2hvjeqrrw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2smrkumhx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kpinhovs.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fykogrwh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oulszeum.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ccotudzw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2uhpidffk.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2msigsqpb.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2kziwgvcs.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ipdxjedm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2glavyssa.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2euugtqkb.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nulzpqki.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jmfszwse.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2teaccjqo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2wmfutxhz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2hhmjnyvk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ikmhpvpb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2hqtvptrj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2yerpflpe.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2lixkjlwt.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybnjlcve.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2fedgamyi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vdfgplkr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2txxsizvi.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2dyturdgr.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2rpbdivfw.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2znnzrsyg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2dgpuoxxg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2erxfetrz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2yezovzqa.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2koiuunbs.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eggmusuu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2llgdtzqe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2cqlylxgh.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2mrjjmbul.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2sdahyeff.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2tgnoqoss.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vvywvtte.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2eeeukwdh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qgcrntti.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qgyatutx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2bseiwufg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zeoqrskk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2imzbwysz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2vcyhshug.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2caaozqjv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kdqdbqra.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2iexjglrl.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjmeuyen.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gbuavflz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ntloqwfv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jxzshmrx.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujjxyuhy.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xhotslgu.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xtpfapld.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksnhxssr.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2smkjaobu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2imxvcpzz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sojujwmp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pntvggxa.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2djrufcvm.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vkkzhqer.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2yuyctemz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2crfmxdvr.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2klpdmkpf.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cssuueqm.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zewanhgs.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2izgwgqso.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2xbmjawcb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2gbrfhcgv.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2ydrfhnqv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2lzcacdsq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2bzesztxw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2tldvxzxg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ldhhqpub.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2quiuvkvd.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uahtoftp.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2qlhzvsbe.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2szuokuhh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2rnvyymcn.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ddzqcwpd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2exbjuhlt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2wgbgcjmb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2xnpnczxx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2iofkponm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2asicrrbn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2azqknhcl.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ezctsuvy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ukaeiwmt.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2yjiewaed.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2gubexpiu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2zdohgkfk.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2crmgwilb.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kejdnvgq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2adfzabqq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2wsbnoqse.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2qklslmbk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2nwtokzwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zbwjkbgc.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2povannkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjsybjrs.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2yyldfhvv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2yptdqufg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2uogspobq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2eolhzhcc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qycegoes.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2hpottqov.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2kjezomxr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2prswenwj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2gwlawpsp.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2tojvrwlf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2sjfeplht.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dpmpvmsg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hykrijsv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bovvuedz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cgatsymp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2lcoqzmqm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2xuvcbniv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vuhawgyd.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2bifdsysi.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2tgyzkhzj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gisidwhl.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2eoqjvawy.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2escfmvfx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hctnewvb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2xvcpzorc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2mxmkunxx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cywyegnf.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2zffcuzov.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2uygiytpo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vndwotub.html


<!-- 参考信息 -->