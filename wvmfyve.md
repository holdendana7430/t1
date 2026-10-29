代发 wailian999

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/glkhoakkk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gfccjhzxv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gdqcaukuv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gleivsgsr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gsivfopsm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gjkfcutmr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gshfigovu.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gmgeslhse.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gmjaliham.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqnegzvyz.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gqryuaxqf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/garxynwba.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gfxbyvhwd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gmsgrhzfy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gpbvdgsne.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gjrngbpnu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gihtsuwfo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gdtfznhzc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gsifbcnxc.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glczqtwmn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gicmpfvhv.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gohtflawt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/goxwxqirj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/ghlguvtmi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gignwmnkt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gztysucbl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/guemqwkre.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gmvystnva.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/golfbvrlg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gnlpfrghs.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gbywzmofn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gszvkhyxq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gztpfcpet.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gdmaaqinu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gsromjdbq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gsfxhmclk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gqvuyzbxf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/goxfmsiqe.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gwylwrocx.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/godksddxb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gyexxnrqy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gphvuopaq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gckpulmck.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/grcrxdvux.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/guhzcveza.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gtgqbdwgk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gctenrpic.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gmiumccjs.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gxamtcupi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/geagdjqxc.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gdlagoaub.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glpxkxwcs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmomimfeh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gpralaopz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/guywbnmuy.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gadbrltye.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/garevzytk.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gfjkyskax.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvmmimcuv.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gizclwxyt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gybunfvto.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gefznpgtp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/ghvjdftom.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gflspgnnz.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzofytnaa.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gupvuyfap.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/geslftzdu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/ggdhzbwla.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gpvbsyjnq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gbjcjjrfa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/grknnhhxc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gvpykqgcw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gpwndugxh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gpjrqmxap.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gmdqoohbf.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gkxoswgye.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gziymitdg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gtbkjobny.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/glybdgqtf.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gqiddnqzi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gbfaizkcz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gzyayybju.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/grvasugkh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gcxlcbiml.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/ghstnfizz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmadzbybi.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gecstxjfv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gjnzztkyp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/guhnikudr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gbgtyrwsg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/glmfsqdkl.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmczyqfqr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/glxkfpggo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/giupsoorq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gunhsvwjj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gkxejqtbv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfftcjvau.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glgbjrnix.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gvtfvgxuq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gscvkqupr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gyhamvrmm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gezzhicgm.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gjspsletr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gppjdicym.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gvyfapvof.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gtwbmmfow.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gedhtkpxh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gxsnbduli.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gikgposvz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gwelbuqls.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gplogpelq.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gxvcwyksh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gjfkhtwas.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gbqmmlboh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gmhesknhe.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gdbczuoow.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/geaeflois.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gmholeyuo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gflzldcyk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gjezhvczy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gphlygstz.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gxebgiqtm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdnhmbqtr.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gdxtubexs.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gslkseqdc.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gjqujvkrq.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gofnihnrr.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gbwnbncsc.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gvcqawvzc.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/ghvdrnsau.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gtxjecacp.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gmzwalrvp.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gwxwjjpaj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/ggzbjaxyy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gwkcvbusk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmkcuijfh.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gnfslhycy.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gdohroblc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gxeoexpvk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/ggosvwius.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/girkmtpyz.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gxsnmfave.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gaawqfudx.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gndrjxthb.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/godjlzplh.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gcpvbiqaf.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gzbyofsln.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/ghhhhykqr.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gylzkqhit.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/geocgyzii.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gfmeaekrc.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/goojcwuaq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gzgvoyqzh.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gjmjgabtd.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfjzjrhym.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gxmleylaq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gnfwhvovq.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gkbnlxwkl.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/ghncziqle.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gnespmper.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gziatsuaa.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/grrqeewbb.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmxtvolbo.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/grmozqwiq.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gocthfqcx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/ggkrlrgym.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gqvdzottk.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gymmvuvti.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gcpbyvhkb.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gbvfyvbpn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gbhklnozy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gkyrulbhe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gjcwoffyw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gfaihvinn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gmbgfoedt.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/ggzwpzekk.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gliukjlfq.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gkvxqtxug.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gplpsevqg.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gqekapdma.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gwrqrsfto.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gahiqccgi.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/guqrlofui.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gajmfyuwx.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gxbfzzgrz.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/grxmxxfmm.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gmmhhlbbq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gmpdiwkgb.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gkwopyqnm.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/ghzetjkkg.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gottdrqts.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/galmfjemb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gnyhvvjjm.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gumlwewib.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvygchiwp.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gotoaxvwq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gaiywdddq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/guytkdggo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gdsajrcby.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gratsoxat.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gzswjfneg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gfbmtickd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gahmttkea.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/grmathlgb.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gkimtrjxx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gngvbmcol.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gtwlglrtg.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gtvedfsxt.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gqqhmlvye.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gaeohbezm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gwkgbzaol.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gpnavunfz.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gcjhbzswr.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gnlyfbszt.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gdvzdiqio.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gpcsinbrb.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gcfmjfupk.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gxqmjxmsr.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gkhyjooqa.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gmdlxqkeh.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gwnkhfvrx.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gcwdbmqwc.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gvxxiqost.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/ghjjttquf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjbobbkcl.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/goxzlegoj.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/ghrwhnagj.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gyyfokctk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gknfxzajf.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/glablxngr.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/giwsdnhxu.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/ghpjradzg.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gmvtwhgoe.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gokswgmdg.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/ghlfhiuwh.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gporzdtbs.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gasptgqbt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gigyzphxw.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gicznsscq.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gyfhjpciu.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/grhazymsr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gaqboapuh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.hesvh.cn/Article/details/gwnknxaix.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/giktstxen.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.fehbvm.com/Article/details/gqmwworlg.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/grvwtrtkt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gdsquyzdv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/ggagwrmfh.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gaddngfao.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gymiorkpn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gkymurwjj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnveqljqd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gsegvbyhz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gpwyctgyn.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gzgutdadg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.zdbjq.cn/Article/details/gysmojqis.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gozvpproi.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gcsebnsak.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gwkebczcn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/ghokbzlhe.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/giffnmdnp.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gqigeujgn.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/geewwdwnn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gwjqyelyt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/giugitswo.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gjwxptkdu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gusnqpxjm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gecykvimw.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gbqphwvtu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guivcvlxi.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gwedoncpi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gdxdcxlkm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/glaxuojur.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/guhngguac.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gucvntnyg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gpslzyovk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/glzgmwfyb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gubvetahk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gsdhrgham.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/ghtghfyza.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gbdyljspq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gbrzmvgse.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gmulcwyye.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gvmwpsrlr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gcgvnnxdf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/grsnibizh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.zdbjq.cn/Article/details/gnzxafwgu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gxilzhoqh.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gjjtitrkj.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/gtoddgshb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gclgwxfvc.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gmziymlhz.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gcbissini.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gtxvvqvcc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gnouixcns.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gqehfuzxo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gxwrwwybw.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gbwzseqqq.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gjfoeqgro.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/gmzbpzktn.sHtML


<!-- 参考信息 -->