代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gkmgyjktb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gkiaaycel.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gypedgahv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gefdupnqt.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/grkeoicoh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gafmngqhs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gilxpsvmn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gyfhempkn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/glwwbabfw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/glminzqno.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gqpouqzze.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gkanrmthr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/garrjsyty.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvpdopocm.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gztgdfujv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmouxyicv.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gyerpzsnv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/ggkvqtsms.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/glsyxpsbs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gabzyomrr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gsptdnqns.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gfkvznokd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/glquupcoe.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/grrwwmfgk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gvtxkijsh.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gjnyvjpxd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gdvwvwodc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/guwiorhtv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gzucgukah.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gnteqqbra.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gctprvyne.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/goiorwdqv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gxbbsuhbw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gkpwvgbmv.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gntluiqrh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gdcnjvdbj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gmfzemfxl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gaighsldi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gqmkxbrty.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gnvfdhvvf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/grvzysvmj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gvmhgtaly.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gkmflfsme.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gepivrcch.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/guzmvxxys.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gmaynlfdk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gfhwkypzf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gjjbysvfh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gytvfpbst.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gxfwtzhic.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gimbfstex.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gnjgzhjbo.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gucbalsnq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gynspuecq.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gyczzdott.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjndjxwqy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gqxwrvcmx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gvfhaatoq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gmqkkohnc.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gjzryhxfm.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtasdbnjz.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gluveqtoo.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gfhmzllxh.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gfvdupaay.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gcngagxmm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gksimyvcm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gbsbeqhrl.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/grlgltbjf.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqrvjebkq.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gdvgnowzc.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gebqzgbcw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gwqigesvi.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gtqggvobg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gyjcxecef.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gwyxzgoyh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gmxosiysn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqtazccr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gabkdyhmm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gfdhbfoup.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/guadcrnky.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gfawkscyj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/geyjhjatn.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gzuuvaion.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gxeajvgeb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gzbdwcvem.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gbuaqebdt.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/grscmdalf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gtqsormqe.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gjgxtixaw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnxzmthkk.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gxjhcctaf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gvgsqudsi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gggykjehy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gtwsbeivt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gtsggqedk.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsbylzehk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gevdgyyhz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gobhzdqql.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtckjhcdz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/gqbhxfzfa.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gprpvkjhh.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gprnnhijw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gfindxirw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/goqjitewd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghaygfljf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzpcfgiwe.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gdwozdhrz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gdwxhqmjk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/glnaaliki.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gatkxlwqw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gczkhqbza.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gpxwzroal.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gblgnhwtm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gtfhldkdi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/giihgfjut.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gsbzdbmdr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gasvqchxt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gwqasrmlx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gfstkhzto.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gghhllfcq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gaumrnzbc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gcgdsraod.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gnrvggjou.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gvpzazejd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfoaogmbt.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gtxwyskti.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghdlszyid.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gneyviwor.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gxegswrcb.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gegpmlhja.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/ghrwcrtdh.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gbukigldi.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gjptxfosv.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gyxjgswhe.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gfzejoqrp.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/goiljouqj.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/glqeksrqb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gzxecuahh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gaakihkor.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gvslihqwp.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/giliemoic.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gsqtajsyp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gaorudhtj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gspvcjnzx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gubytvzui.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/glwspigoq.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gcwafohkn.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gogpahxgs.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gehifparv.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gelhgspbg.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gfbpivmkd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gamrjmlud.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gspjyfzoj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gwgkkauxy.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/glnwbrasu.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/grrmihqwq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/galjpmnkv.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmolsvyqv.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gbchompyy.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/ggoipmyva.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gzmklcglh.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gtkdiivyv.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gisirzbkb.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gogfzowyc.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gelclgais.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gqgwabnpk.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gacdvatlh.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gabbdganb.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gboqqjrkx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gcgyoyjym.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/giteskeso.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gijwmkkfd.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gczuyzsmp.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gxwhsgmed.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/guhkxsqzp.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gctqaqfux.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gusrpgjpq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gexfginok.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gzlqqulgs.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gbrehouxt.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gsipnmceu.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gzruysckc.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gkbivmitd.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gstubcbzw.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gkwvajlei.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gzngrzhwa.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gpojlsaou.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gtzwldnwp.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/grhpsmxlq.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gqirbnsrp.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gwbyonrhz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gytuypngn.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/ginxfrsbe.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gjnwnqqvf.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/grmqtdzxv.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gmqiernkt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/geuzyyros.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gkhscdmhg.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gdsrdfkwy.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gyqcckygt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gtwkdhclc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gdkotjzwl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gqghvahhm.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gpogsjzeo.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gjrnctuvs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gpyksccps.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gcpsomgqs.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/grjvntsdq.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gapfcvtpy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gxdxlgcqc.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/glewvjsoz.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/ghnwncguw.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gaykgtaxu.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gmqcuddtc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gxnblbali.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gkqatdskq.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gceupmrcj.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gdppxfirq.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gszlhqtdk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gvjdzijch.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gynhhpbtz.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gpdronowi.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gtjgxbdwm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/goqjbmduz.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/ggccojmad.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gbpxwykbl.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/ggddnkxjs.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gvqubulex.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gciuakgej.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gbhcscufw.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkcpsahmo.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gptztdjfb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gdqhkixtb.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gpoxbgmyb.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/grkwxmtmg.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gqnkmrxzp.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/geqkzqmrg.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gpdjofwsg.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gdavvvtyn.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/ggcxtaene.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gvlfjmnpf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gjneqshsh.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gzqxtrauj.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gqgfoydwh.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gmupxvbvu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gtdjqiyqk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gethjnovr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gejwcxjaz.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/ggtpfkpkp.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/ghstkrhns.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gdwffciac.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/giddamcen.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gfeonzsaj.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gqckouneo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gqrqluatx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gdbvrylwl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/ghnoxequy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gsxynulnr.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gixyvgrqz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gjoorddbb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gylvmuwzo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gaofzxqhm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/gnobdsofl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gcxlanmcv.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gmynprumc.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/ghgnuokbl.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gcemorcoy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gbffqmbcu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gtusubrcs.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gnuvzacwf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gszxkxzhs.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gygtgsiwv.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gsttvpcgn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsbsudibo.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gvlzazbdw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/giqybgefz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/ggeozkqwt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/greazawdz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gdhtogegl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/gszjazbki.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gqmvnednw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gcavlpkyu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/gidmihtqo.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gitmsdbar.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gkyfrcbkw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gtdgvloxy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gnflbleti.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gzubvkelh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/glbolmlne.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gxphudmxx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/ghqhsjbbh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gidceyrco.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gwtjkidxz.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gfyxesukt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gswxhyblw.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gwdlugxga.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gbgizatjj.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/giqbbximb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gtjlwcbad.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gskujhwhq.sHtML


<!-- 参考信息 -->