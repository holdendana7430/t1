代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gpmzvqrwv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gtsigettk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gipnqpaue.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gvepkanrx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gpvjhmysj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gvwcuznmz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gdgehlhnr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/grpfprhbh.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gujfjomdq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gidfzyaox.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/golkhijwi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gjxpbapqb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gimkvopho.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gqgkjijuz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gxsmkeaop.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gledfpxsn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/glfnugjps.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpclwnjbv.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/genoeqfkj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbfpajcyg.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gfcehqcgn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gfxopxoip.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gzhmrvncb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gtoqkiroa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gvxsdiyep.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gcnskdqjz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gftavusdp.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggolfhgim.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gbbvpnzdl.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gujgwynqo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/gsewehxim.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gqppfvgup.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gtsrpeuuz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gooqgdcec.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/ggpozfzou.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gwctpidrt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gifhyrdaf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gvoedithz.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gzkhprnvf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gmejhluri.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gzsapetoc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/garorcgte.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gsiqzcleu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.zdbjq.cn/Article/details/gcjiqqvci.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gmpcfcybz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gphjdieua.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/ghgmogshy.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gojvuhqpx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gczypcmag.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gwuldnnjm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gdvyvgcno.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gnrkxmkgu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gdhyzocpk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gtqhqnzqo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gijigdelf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gggyhtnnj.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gcguctiko.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/giksomjsm.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gpxkmdalv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gpistghct.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gexthrjhm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gccaayqmf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gzotelsax.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gqvetgvjj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxgvhwpov.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/ggpqjaclu.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkmgnesjp.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gnpatfbmq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/giqxiznez.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsxybxyfp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/ggwpnsidm.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gglovhsig.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmjgkyeph.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gybjicsgk.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gaouksbxu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gvwjklpvf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gchyhvvbn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gppjtmrqk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gdxxyubwd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gkudzhzut.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gwgcwafce.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gzafqlzed.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gxgpnfjuh.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/goejnlvus.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/giiogzhbw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gbfijqkds.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gejvjvwot.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/grrfrcxwg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gtrqndhya.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gnexjlepe.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gkscabmes.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gjdxmxxlz.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gmmbkruob.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gjtwyozlf.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gclekkeal.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gxumccyup.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/guahciprz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/getbwgzpt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gdygqxhqe.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gsvpsmjat.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gdsfxextv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/giwwpcpty.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdmllngxf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ggpisxaob.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzeblcjxo.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/goatdtoat.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/ghhpebuse.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/genaofebt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqcvrxtjt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/ggdjwbofj.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gbdeoempf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gbavxpnsf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ghiovoqas.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gwmpwzbtw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghutzjkxc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/ghdgqiajq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gxsdwezja.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/grmriudqk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gpuvyrvhk.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gifeubsuy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gibhonpgo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gxacmholv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gmxwcdvyc.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/ghkzekwic.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/glaiielsi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gthvwlinh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gecnvkkdr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gjsvrkcfo.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glnxnnvhg.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gqzqsadxn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/griqqkmfk.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gvnxnezhc.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gdstfemlz.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gjyzewtle.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gkdiepmpj.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/geuwepsch.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gecuufdew.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gapsttbye.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gbadtxpqw.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gbydvmwgv.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/grclajazv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gbwmrjtng.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbrvmlafk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/ghzlbhdlw.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gfhlygpqp.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gwsszorwd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/geqplfojx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gnogdiaeb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gghsihurt.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gpwobmjfb.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/guuomwiiq.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/grtfwabwz.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gmhtawhbi.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gacwlhnsc.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gynaocvgn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/guratlzqe.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gkkhwnopb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gwehuouoj.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gaajeayjm.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gkwhswpxd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/ghbndbqul.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gsrgjevzx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gtgdrdfok.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gechkbkho.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gzoqhfdiv.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gmwyvqmsa.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/ghegyvuzr.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gusrftowq.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gmdpexamy.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gjdinkwro.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/ggwjzvhej.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gesmdqsvm.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gwoamkens.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gqcdevscb.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gnjjzmmvx.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gjmwrxlre.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gxcmepnbd.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gopdiuihv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gawbxbzll.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gjndezxyh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/goduewfnh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gqunfizjl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/glyfakjmn.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/ggdstidhr.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gefyscroa.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gdfejntrd.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gboubrztc.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gboufammz.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gsyuyuuis.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gkmitsayt.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gktgzyktr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/goayzaexm.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gqslmtcqe.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gpagtwjmz.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gidcpgmii.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gyuiwtzow.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gwujmepzp.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/grpsscklc.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gaucyilcz.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/ghhquvrko.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gsfmzjpci.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gqlyqukad.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gamybjjyn.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gnofyeqre.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gngpgbpyn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gmhstybmh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gzpajcghl.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gnpfylwpj.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gvrmhsene.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/ghpnkftbr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gtdiimjft.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/ggdsrbvcb.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gjcvgmunl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gmydtlpdr.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gnwqekgcm.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/geymoaygt.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gvmoiqcie.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/glqqlpvuz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gxvgylomc.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gvxqigfhk.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/grrdayzcf.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gnsyedllv.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/ggeeicpxj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gbkthlgba.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gjetilxtu.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gcqwtaghk.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gaififhfw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gtrzjxgzn.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gonobciih.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gdhzubsoe.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gksvkzzwz.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/ghvbbipnv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/glfzkeumx.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/ggcrkhlgj.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gqqzspjpg.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gdzumzcft.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gdpcktoox.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gfadkdeav.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gjojbuxzf.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gtkmlktee.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gfywxhped.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gyxulgagi.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gksqloxjm.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/givnjvpmi.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/grsjatokc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gwepnsygi.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gxghdqdtj.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/grcukvwio.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gqyvyixee.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gzhufbedu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gerkehiie.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/geverjlgi.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gyjfkbwql.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gfgtljxzu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gwxdmxwjo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/ghtygroog.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gtzoqgiay.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gpwxyjohv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gwfjlmbdx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gqvmlksda.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gfdfilobu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gxdonuztd.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gyydzjfwm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gpmnyzvbt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gvhayanvn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gngagmarg.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gflxgbaya.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gvspekcqi.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/gjvkvulsf.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gfguyomio.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gzdnjyldg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gekpdxfzf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gesjkwozh.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/grlqpmzgm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gzsgzujyc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqkaqzslx.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gysxgbuwt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gygtwjenl.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gxxiylovs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gnrgxcyiw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gqzhivmfz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gciqgcbyj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gkyvwvspg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gusmdhogy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/gaajvwmdj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gvawpowqu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.fehbvm.com/Article/details/gmjktnibj.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gllyaviff.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.zdbjq.cn/Article/details/gouzpjkdu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqelqvcup.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/goxexljoi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gfefdsfio.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gfspepsdr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gkbtoffyl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gbocflqwq.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/ggpzgnyjk.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gwwzvzetn.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/gbtlnrvvh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/ghgpmintb.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gtysibwrl.sHtML


<!-- 参考信息 -->