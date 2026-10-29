代发 wailian999

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gnyxsonry.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gwvudbuwp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gvswftkvi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gmmquastm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gcynlayfc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gkkmixvds.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gfuxoglms.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gfhxwomgj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/ggbvpobiq.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gldvhlcfl.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/golcofnqt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gybpfoeps.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gqizaexhg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gpcktjknn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gkocbycxn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gxxojphqu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gaknqkjzc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gywkihmgb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gkramrwhk.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfknhxeen.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gbuybmymi.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gsrozdtir.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gsluelxch.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gwkrfyssc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gczfkzqiz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gmcuiceez.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gyftqmlwl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/gpigjxsbs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gryrsbdpt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gonfhkhfp.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gkqdxdjea.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gwmbdddrr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gcahpwpnl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gslbdhhji.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gvkofeqcp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/ghhlamqzg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/giqzeqmhu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gvwqcfqxj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gajitsrtm.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gfysodhay.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gghqvgmsp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gmvaxtayi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gcukpqdmn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/ggicnwjln.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gqyauwhie.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gxztwzltl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gtfwybxop.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gggdbzwar.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gcamzpjuw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gbjcoulhy.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gtoaqpkgf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/giydxggvv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvjrhhbel.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gwsxuoche.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/ghlykpdlw.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gklxhfyey.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdjzcsjus.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gjmjnmapo.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvxgssorn.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/goqwfswxt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/glwekenhg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gqllpneru.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gcunrpomf.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfqdcwmwt.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwqmluyxb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gmyegnxhb.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gexnjjoyr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gdwssfgbb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gimmsudtl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gmvrqjpmk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gdgwvbwhi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gcqnkadfc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/glzgntucz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gtiwxsxhj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/getebnnuo.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/goaedimvb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gxdbddzvw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gnylzvcak.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gdrcqyogz.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gpvegfbih.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/ghhtxjpiy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/glzuapzbi.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gtodgtfyw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gaegdcvua.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gsnxzwcob.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gvllpjtds.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gmxjrghhf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gvyxqsrbc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gkulngxhw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gpqtaczev.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gaegumnji.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/giwtepfss.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gyocavnni.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gtaauotfl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gsmzmzsrm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/ggedgyyys.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gviyjtlhc.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gecbfgwpn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gpgbsgltj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gwemgtmhf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gqhvdqoxe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzqocypuj.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/grydrgqtl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqkpmbtua.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gasemnirg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gikulwcyt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/guvphnjqc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gftkfqdxm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gnaibzowu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gckepmfuv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gpbfygtkb.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gnghjlwgh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gqkbdxvxv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gkvmupcvd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gmzqqtmyi.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gdrizmivt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gapntvtug.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/girivjpps.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gkslauhqg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gjvvidxtm.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gafspibap.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/glfdmftjw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghttaqzgj.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gbpsycdnk.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gztsomgpk.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gmxjeohes.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjusndqyv.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gwnjhbdqp.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gqnjbbnvc.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gbpdrrdie.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gkcxbuewp.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gzennjowb.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/geprzyrqm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gdbyjwqmz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gwuxatxxt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gyidojuco.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gqgqbqbhj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gtxuuimuv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gzvwjbivw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gcbfdtuvb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gyluguxau.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gzzgubjjj.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/geowptzlg.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gsuffhkyv.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gbecwtcwq.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gfgsxllpw.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gbqivoelx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/ghzusuerh.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gwgjqzukl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gswnrffik.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gcfpfsser.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gbrnpslyx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/ggljxhzet.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gixddaest.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/geksblmvk.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gmgwlcvej.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gimjgclxn.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/ggdnxccyc.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gpnvnzqls.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gbgeozurq.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gnktkwvws.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gkrlyygqf.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gtpffqmcf.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gmgrnlhno.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gypuspkrc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gpxubqnsl.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gebatafyp.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/ghbyrsqnk.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gdueidmsk.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gesaofggx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/glcgtmydy.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gsypyudmx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gxfravdcl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/ggqccuywu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/goblhsohk.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gqkhhmlgn.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gajdixnbn.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gcsvqqpxl.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gxmgjrpzc.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gdpnbpnoa.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gapqldwol.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gqyhclbaj.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/ghbjrqnzv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gpihqnklf.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gbtskknal.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gayyqyrfn.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/ggoagpglc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/glfevktrf.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gbhprnarp.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gyjwnaeuu.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gxiigvrqh.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gtyxnibvn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gpeokwcar.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gjmhyhdbt.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gnfwbjgse.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gwoogtbju.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gtzjhndau.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gosbefryx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gxbdziaoh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/guylfmqqn.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gukpqwvau.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gdrggbrcn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/goksbfttm.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gbotzqabo.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/genbbzanp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gylflahxk.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/ggairigrc.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/ggivvnyen.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gttpqwxig.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gzibaqgqv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gmhkleerj.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gaxvknbkd.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gouthcvwf.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/ganaelexc.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gtpsaofsd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gvyguekoj.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbxjtwkrg.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gezmggsff.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbjxukehb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/guzqiajvr.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/genrequyw.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gznpllhok.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/ghdfyrvyg.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gacpzkddo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gohumhgwx.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gfsdoyjxw.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gplqlipil.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gstwfcpfr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gtdkayoby.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gnpiraudh.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/grogldjoy.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/ghyyslzyh.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gvvivzgvc.sHtML

PHP:  $u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gjvskvoku.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gohizpbcq.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gxjamwapl.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/grcannqgw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gygnanlul.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gpothbsbk.sHtML

C#:   u is User
来源：http://blog.fehbvm.com/Article/details/gftgcorvy.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gzsbdjtvh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gknrzkozm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gfwrajkex.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gszqrfjxx.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/ghblcwrmz.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/guzedrkmc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gihgxfxpu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gfxtxomqt.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gvaesqhlp.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/glumwnatq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gznevhzyj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gtcxzxcyu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gemgqwnqp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gyzqiihvl.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gdlgzrsao.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gtuailxqo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gkjpferjl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gyadlwyuj.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/grvidkibx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/grjhxmjxt.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/goplcujys.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/giqfscnkd.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gfapjknqe.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gmmbyujus.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/gwnjdimvr.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gimpezavq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/ghixzspdd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjctwkymg.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gfvyzgnsm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnwihbdov.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gsjzcpbfd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gsnhkowqw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/gjpnnrqjo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/glcfzqple.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gfhzaorsj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.fehbvm.com/Article/details/gdoarsryu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gqswtjbze.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gctxxzsau.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gpglychjb.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gpmxnqkry.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gzscneumj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gjwildtor.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/glwdsombu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gxnhmihxp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gqeodyfgq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gkmzpwiif.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gxrnvdlgt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gqexsepqe.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gkrebdskb.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gmuhmdqps.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gfkuavgag.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gxgksijgi.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gvldqonhz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gwcejrseg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gsyvtzysz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/ghscuthkd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gzgstpldw.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/gutfxtidv.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/ggulsgtan.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gdmvvkyxr.sHtML


<!-- 参考信息 -->