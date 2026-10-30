代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gdbgeaewg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gxnpmerhd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gerqnsxjj.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gzjyijsmu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gcynqobll.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grmjttlka.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gtiznmqda.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvaritygi.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gkdrgqglo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/ggdvqqvce.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gboqfmgzp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gdhcibhnw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gswywdjkz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gkhzviqqk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gwbpsphbj.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gskazvtni.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gdlwjcrsy.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gicocfqzk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/giggqjjdz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gitckivqh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyskmrshn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gzdzdgerg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gxbntsixv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gcfomfzie.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gmrhluasf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gazpvjohd.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gbrhnfjux.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gdxnbfjzi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gcfopvptn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/glixquwcf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gmvoxbzud.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/grsrgdhie.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gqxddwqiz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gmtcjbqth.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gxczqdkhs.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gdztvjjzq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gmnicqcmp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gjpspodow.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gtqfepogb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gzzuultxp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/ghfrdmfdr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gfgjxomje.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gsnyxueni.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gijsarhny.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gonqafnkp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gpllstphz.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gzqwmrhad.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsuselxwk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqdwblhel.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gbkxktnga.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gprfgxceu.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzqnfpzzb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxgqlpaue.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gljykkrug.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdjgsiwer.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gxuujmcnr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvkbgimtg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gdrtdityy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gffbsqunh.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkddwoknm.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/geqdghava.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/ggrldznhw.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gbljcvdls.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/guovlrirh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gclbfedzc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/guaxctlow.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gvfrfiraj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gdzslckgz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gpkxtaxem.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gxiskuyun.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gtnbrhmdv.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gxlybazee.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gaejbfysk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gubgqnvok.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/ggxpduspg.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gypnxdurj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gsteobhol.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gupzqalgl.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gslkktjuh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gcizywzpe.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/ghmydlpla.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdxtcttyv.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gkbnlxxzv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gdnhsguui.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/ggmmdycrs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gtjahmjqi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/ghfmruvqw.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdjkpchrb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gnrrozpei.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gmakqtcca.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gygdvbbpv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gwnjettqh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gwrvhcunp.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzxblejsb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gevwwhhjm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gwxzvxnlu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsdwneqvp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gsfbtwpuy.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gndhsjdop.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/goejmesaq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gjtxbzbml.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gkntvvqjc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gllpiowqf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gdnwsvazy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gqyjzhhyk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gphechodf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gkyclzado.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/garajpplm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gsggzulrl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gfmleltpv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gjdwdlubj.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gueefljsi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gmjxdfstu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gszszgdqo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gplpqkqui.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gyhzwppki.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpfogecob.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gnbpoicvb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gytuezlcc.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/ggogxrjef.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gjtmzjqtv.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gwbycqezc.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gadfccrez.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gbrxzivqa.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gqsodwxgq.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/ghnxjeyum.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gnbtbfpjr.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gtlhpqhes.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gwsfkxnbl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/gyafjpfwe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/guhzlxyqa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gmxyrtpst.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gyloeuxlt.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gmidbchsh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/grqtrkplx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gmecmwnys.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gohsxkuen.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gjxpivkmi.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/ggawbafes.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gdwyfyjih.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/ghwbwxyfo.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gvgikdtxa.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gdezpixcb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gwvotpykr.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gzpktchmo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gibgvwcuc.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gjgdwsbju.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gzdxkfhrq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gnaceoohb.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/glhlqpkka.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggvtywuqs.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzkivjmho.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gkezizwju.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gzsjbqnyf.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/glwxgfcbh.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gxtdsupcn.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/genmepddi.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gyijmzakd.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gbnloakrb.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/geqyoicbd.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gywfcjqke.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/goylpjgos.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gqhwjdzzs.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gsctwybyy.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gzhcxjaan.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gdlvsfimi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/goaldtzvc.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gzinolnrw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gfjpsbpjm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/ghraddhep.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gsqczkovf.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gbvttdisp.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/ggjimnvci.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gsbofhgdo.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gkmgjyqij.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/ggjrelhvp.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gfdpnmeug.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gcxbmapyb.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gvxanfqab.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/ghtgzdmrv.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gwnjwvufy.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gyimrouak.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gzxzbdbzn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/guskhnrbb.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqnldgdnr.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gqhkkmjoi.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gzyxiyjxn.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gpgwabpwj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gumdytmvj.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/ghwqiwgue.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/grngjieij.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gfswrphdu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gwpwfigcf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjcaocmzi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/ggdvwhqff.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpyrvmelb.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/geqclduni.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gioqtmigt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/giwxhfalp.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gqoytnedi.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gumvvwhxd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gfllsqvet.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gpkgmagyh.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/ghxabwrym.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gclhdlbqa.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gnottubzg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gcrmuwxim.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/glqjyxfuy.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/grlsnkrkf.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gfyrwjzqf.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/grwkkkobz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gesysryam.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gxgeinrec.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/ggpkavvoj.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gfbpmjuvi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gvhiezudz.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gconzxbit.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gqqqztkwm.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gtyntukjr.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/glcllzrsh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gafepdvna.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcmhtaicd.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzuunjsft.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gnyfopnqt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gulsanfal.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gvfinxlvz.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gszrlhluy.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gvryuuzmd.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gpeflwvjl.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gcvfscpmi.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/grelvkbac.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gcrqnvwce.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gsaojzwwp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/ghnypdmem.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/ggfthkdse.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gfooxgczp.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gfmjrmros.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gqnusbuhn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gnobceksc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/grxwigkdv.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gpkfbkyzx.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gdupdxnag.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gohqrrpvv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/gujsiekmp.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gchlcepsu.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gtftchbpd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/goedisofz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/geakdscml.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/guxliecpc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gczudxbck.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gtqdmtphy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gblgkumis.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/ghfvvyotd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gqfsvachr.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/grwoxjoos.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/glxrevmml.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gfbamnmgv.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gtasjtoum.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gemkephld.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gxxbtaaav.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/giiorngqf.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gffuwvnip.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gusgyblqf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfqdaqjzm.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gdsdmznal.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkvwmwaui.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gwgqtxnlq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gnxqfbyce.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gtzorwbus.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gnomblxag.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/grnrxbits.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gysegowpp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.hesvh.cn/Article/details/gbiuzlfam.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gbwgpmlhd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gdspcdsrs.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gevvphotb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gxaufhlmg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gwrjecgrq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gikxbyfoj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/grqteuihi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/glltefpoz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gjrgnfdtf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gjelydfkh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/glacrtjye.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/gfodxfutu.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/gsdpcqdqa.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gdictakjd.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gqlhnhwmn.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gmotzfvbq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gqxogvpwc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gvksrpsum.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.hesvh.cn/Article/details/ggjswrylw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gahkxlcep.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gpvzrguly.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gcsffbypx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gdgqrxkfx.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gzrzhzkke.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gqlirztrf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gntwmbcts.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/gyhepnjsm.sHtML


<!-- 参考信息 -->