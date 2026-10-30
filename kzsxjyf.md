代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/guyeybelf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gvviefacv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gohoivbsa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gjesfzrlz.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/grqgzvquw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/gosxzmzlp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/ghaouldke.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gwtkeujki.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gvkxszjbg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gcrxuieyi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gozdkcwbq.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gopclafbe.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/goebvtrxn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gxkkqlkir.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gzjriuijf.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfrvpitwl.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gsuwktdef.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gpqoeyocx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gxlrsvgva.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gcluwxljd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gulosaoun.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gfubmmwml.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gehlwuult.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gfvzwnwlm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/glctabynv.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gojaocxce.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/geeqrsnsf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gyecnefyx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/guoskabtp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/grfxhfqrh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/glcoaigov.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gjuibcvvg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gknyqciqi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gpjuolzdz.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gdrzhwwsm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gwzbtllcy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gvlqdkhxl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/guhlijibq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gnwofkxhb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gbkgybtys.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gxgknmtza.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gggpiuehw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gnmshworj.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gtrdvknvy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gfrtiesms.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gxvwrzfcj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gflhihbwo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gcdunesjz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/geqqrbmyt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/grmrqbjlz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gpwfdlqon.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gpweibzmu.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gbcweysqy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gvbujpgav.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gazfplcow.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjomrkryu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqddlizxg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/girwwhkvc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gfsjblqls.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gldururfr.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkqexrong.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gawhskipd.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gilbzmtqs.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gtxsfathd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gukcdwqyg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gcakfybfe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gcvjouwjg.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmnduflbc.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gedjxcwbp.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/geccllyjw.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gtpktmntx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/grmuermag.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gnppbeoar.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gddprnwkl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gkbsmmkzy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gebiqlyaw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gbejzvcoo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gqkdqvgaw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gsumpgiur.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gqcosnqma.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gktffzgkd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/goaiqgxsb.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gbaohzdan.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/grfgnccez.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gxnnxckyj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gndswenaf.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gndmdzucw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/guqftnjcb.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gmxwqmacj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/guboyfsrm.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gesqhoqmw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gmbchbrtw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gbysvuptv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/ghgeceojq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gvyanzeju.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmsyrkgol.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gcaxfttsy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gnxxomosg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gqwadkran.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gsvvwrbtr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gtfuqihqp.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gkybgkmbm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gbrzvaiim.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gakjauflz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gozckcxqa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqwbtsidy.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/ghfhserbx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/grtuubnhq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gjtyylusm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gfjjydnsu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjdzlgius.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/grjxpliwg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gtrfrutvn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gjxshokev.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gssspbowt.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/giygdvjdy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gfdovvlhy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gshfshxkh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/grtofyshb.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gfrjqaioj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gaivajiug.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gzjzgpdcg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/giqskkbvl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gaovauvuy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnbzxyvbv.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gmplqgrwh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnnhmntfl.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gpmgkrnwl.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gnxonvzap.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gcagwhbuy.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gwbgodofm.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gbmvimhpb.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gbwmqwkup.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gsrxibqmb.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gqucamczp.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/guxbxhwac.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gemempehx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/ggckfoskh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gqufhtuln.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gdoduluux.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmusqewxh.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gjuwrshna.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gxdxzjvpw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gpzoupvcf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gpmjmodyx.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/galutqjnt.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gogldimut.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gqzeiczsv.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gijkahyng.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gjeoniudp.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gpcnfqeki.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/ghhkkyjuo.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gnelrhskw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gjbgojbae.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gyxysdsbf.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gplbgklgv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/guxnprdqj.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gvldbomcs.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gdkihuebq.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gfirmnwjr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gcjtmoopa.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gwvfynfvg.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gkostkahn.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/goofuttws.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gkcqqnxmp.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gmvpkewpu.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gaijflfik.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gvcbdhzlx.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gbetukirj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/grxzevdoa.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gmfcpjwfc.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gutmeaktx.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/ggeccwlcj.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gzlvwvqcn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gbmzeorcw.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gsicujpry.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gtrdgjkcl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/grgcvkuvt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/ghkqbhxvh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gcxhyuzdg.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gxruceprg.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gwmeabjxh.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gpithrrrz.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gnmrcidry.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gjyxiuwis.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gwgxwnnrx.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gsukvsyzm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gvnkodkiy.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gopwrjfdl.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gcfhzifio.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gdfevnszk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gxhyudube.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gflpdxgzl.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/ghoasfkke.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gbojgjtfy.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/ggtxwqkmk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gtecjfkii.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gabpxtslt.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gvyzdtqns.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/ginuokbzf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gwivnzcjt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gmxqaazcp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gvyvchpbf.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gbeokpwev.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gfpzpsldj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gkrmkxbkt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gyaftcbqr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gqyqvdirz.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gdujyjuci.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gzgykeopd.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gngrlremw.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gwqvetcwk.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gjgcqfqwf.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gekynwdce.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gwlxxnmsp.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gfyczpqbo.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gvtbvudnl.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gxcjaupfo.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/ghpnjirkn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmikpvduu.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gkvzlclnu.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/ggwcfziva.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/greeixicd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gszqcfdcw.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gmdoidwvw.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gqzqtufij.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gbqcvniir.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gyrlxpmsu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkuilsglb.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmwdnrhns.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/glgyqkjze.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gomveiqmi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gnmmdncud.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gqnyxztgp.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gvxlxaxyj.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gbxwjihgx.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gofsyzcxp.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/ghqdjrtjt.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gsyiwvxvh.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gytbablko.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gizcieuvg.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/gfyzxgdxy.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gdngboyga.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gblsvufah.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gebqfktlu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gltcatdej.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gvdymapwi.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gsxessgdt.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gbdqyxggw.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gfoyoxzhk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gedjntkab.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gdwrbgdmt.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/ggjjtqhey.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gbwyqpbeo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/getgguwez.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gldxgnddx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gshzuhwoc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gzliqohec.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gwnqvjonq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gqzayksxo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gmlpuyvdr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gnutlmccu.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gepjbskyc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gijsmtuta.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gqbhnluka.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gpgqxyczk.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gbooejcnw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gmhqircbr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/ggyuamzuz.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/grdomynqw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gilixekyt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/giyihchaz.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gxmmdioia.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggkxgexsk.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gbuxkmqbb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.zdbjq.cn/Article/details/gyftckihg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gsjpeddht.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghjlkqzuv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gcqeslnie.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/ghmrznygh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/ghchwezze.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/ghvlqhuce.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gwqhasyqa.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gkvowwzvy.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gdbektwkt.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gzjotofbk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gznzvpgfv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gouipxpij.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/ghqhgfnvs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gfwgiccyq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gfoufowrw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gegtmniye.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/gefkclpua.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gonnvfslb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gefvzadbq.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gznvavpgb.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/giwnparbb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/ggwtdhkqc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gztrutlrv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/goqvntady.sHtML


<!-- 参考信息 -->