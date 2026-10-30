代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gpmakoqdd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/griadwwdu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/gzimoebts.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gtjqrylsb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gzsipazwc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtemqxsif.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gbwdkhqma.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghdfcbzjf.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gxbqaofiv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gpjoorwba.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gatzrykhs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gmmlidufw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/guqryylnw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gsqrrnaia.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/giukinvwk.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtcjmcjrz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gdyzqtopf.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gptiowgzy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gcfjtuurp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gdvdfkvlj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/graqtpkaj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gceqvjynj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gtmvurocw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/goxafwlrc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gqsxcsrwc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/geiridgmz.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gkdkpvqov.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gncpsemmt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gxtqdmise.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gtqakxogz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/geldlxdog.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gdrllouxh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gavnorcgs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gtlxuqmcr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gvlqaspva.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/glcnzniyc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gmbxyvzbk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/ggiscgsvp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gwucwxemi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gyharqgcm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gownshofk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/guppedytu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gubnmkguz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gxriomfqu.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gfffrgaxi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gohkvrizn.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gupjklcif.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gezpbrmqy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfunnzwpi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gxtqusyfg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.hesvh.cn/Article/details/ggymeaaxj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpcobajqt.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gixomizgs.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gmabcbcfo.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpnvgxaqk.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gvjqrdmln.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggxevyudy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbowdohsz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gxnufjjti.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gyaqhoxth.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcbvfjpow.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/geljwztrh.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gtnqdgyof.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gtwivdjbj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gscmryjmw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gfevucmis.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gefhwlmre.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gmkqapuum.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gbepgnlsk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gqkostyyp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gnqphurnq.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/guiiytuod.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/grsiatumh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gquwjzgjp.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gwvfiwklh.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gqslfqoor.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gigdydhqg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/ghpdxhpsi.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gokbxgdvy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gkcnhkvva.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gnbdfdubg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gswffhzir.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gtttiytpc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gfwzkxhsg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/glldblkzs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gsqcafcki.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gaakfumyh.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gaedqplur.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/guijzzvyw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gfogrqeiq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsnamyone.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gepungjcm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gwfcjauzv.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gzovairtf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gfyhqijjk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkrfcmncf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghdkgvser.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsxpevevu.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gziraigar.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gklksdhuq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gtkmiaxfd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/guqrdsjju.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gjkhttaeh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gbudoiwng.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gsjzwncgq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/grvbxlmxp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gbwodetsm.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/girugmgxw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gcydxzskq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gmfqvymcn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gbgoifhoy.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gewxgfvfd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gllqvesdg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/ggetardep.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gcobsurka.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gclqmvgsh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gquvgbyjr.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gzwwldvbi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gitqhhaxa.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gzmmtjlxb.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/glooehlni.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gppgoewhl.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gophhging.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gxyhwlghi.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/ghgbxjbzw.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gieffycfm.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gnpjzmagw.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gsxzfovuu.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/goxjykeqo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gjjtwkcus.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghokebuxx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/ggzjpffdv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gvghpdfod.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gzapbnnmd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gheuzedko.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gpndvmpms.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gjxykczbk.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/goxgfpnuo.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gxxjggfuk.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gmubetrlk.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gcjdxagdi.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gadtazrpi.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/grickpteu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gwlinavyd.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gflzzgyvj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/ggmoykkny.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/geewsekuw.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gpwzafxfg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gctejjyhi.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gftuvrllu.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gsftvlxfa.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/getwialtm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gxgqpimnl.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/grozkdytc.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gafmpahel.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gjzqpiygt.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gfmpblefu.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/ggjzabkln.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gdnkuuyok.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gakkltkcv.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gqycfmjmb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gfzxynziy.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gddluplrc.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gxmzltnsi.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gkrrgvdsc.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gncnjdryo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gmnnwvpdl.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gqslkcmuo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gwgxlaicg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gsgvwlcmd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gjdcchqgt.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/ghfsedmjv.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gtirzqhvz.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/ghdskozbc.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/ggsuiqrgk.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gmfwzhwqw.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gnmrlhxuw.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gkrjshyxz.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gobqsqjcj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gbvxntqzg.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/ghhyewebi.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gqtnarryg.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gnyoqfysh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gbuosvbsw.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/ghivkzwso.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gunfsoebt.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/garxpnixt.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gjmtptflr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gkodffodi.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/grmeqsyyv.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/guirbgvae.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gcfoagfki.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gnfasafzs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gbxqdjpmb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gvhvizvcb.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gbkhskqpx.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gvjlsdkal.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/ggqhsaydq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gnpglmxoe.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gymknyyvw.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gaqbrnedc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gplsctwav.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gbtckqolf.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gdikudtyb.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gefldgbql.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gnwcqkghv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gebuqyufa.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gjagzuale.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/giomdrnds.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/glxweieor.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/ggmcwhdll.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gfgmqnvll.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gzcrjeppz.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gqknoogiq.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqklsisyb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gnxlgqisg.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gjzhblbui.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gwrcasuyg.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gwtafmskr.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gjqeldkwo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gvkghseqy.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gbvbdpbhs.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gtkrfagiy.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/ghbimengt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gvwoshncy.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gqzmhzizu.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gcdcikazg.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gyvvdwxkc.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gzqqqwqvy.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/ghqbrxose.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gyyjjmesf.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/geegrkdsh.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gjgxqybud.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gezadanrq.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gbudfdrtk.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gyimlqxbh.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/glverdsel.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gylcyinku.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gstjpkzeq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/ginqcjjpf.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gbuekvczu.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/grhyyfgai.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gvhrhzixj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gweimigso.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gfngkapbp.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/grrqxfeiq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gjdgfbsre.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gljozdwmc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gjnfuqkqs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gpeypumjz.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/grqdnferr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gvgamumcf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gvpgaxrep.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gzgrxwebq.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/garlgnnvj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/ggybpondb.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/glagudjaj.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gjaivweac.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gxvxkuevt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gunemsbcn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gitujuost.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gldkxudfd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gcqzbsuoi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfqtfovfk.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gfyszcakx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfqdngkgl.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gapqtrffn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/guyxvfbqv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gqpmfvaah.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gwwzycgnm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/gfbpuqfqt.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gygzejwhe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gbcywuhge.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gyjgpsfjl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/giywunzby.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gzcfbzhdk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/goatmnbug.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gkzzcosry.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gakhlarpk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gleudipni.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gdbbsavpy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/grjajbobr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gfrsmonqz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gumblxxzl.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/ggyzfovgz.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gmyoawxwb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gqlalnlzd.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gagvrownf.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gizwvrmkr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/grjmvpprx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gtwbnxkhd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gtawjzpdt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gqmtqkhnd.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gjejpbtkr.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gabssunpm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gnxcnfrau.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gxnjlqvcr.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gajexkzqe.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/grqgtkwft.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gwcuwxcif.sHtML


<!-- 参考信息 -->