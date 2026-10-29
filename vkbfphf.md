代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gncenbggz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gdjzgtgra.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gyzyuwtre.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gapyufdem.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/grzneudzl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gpbwxurxc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gnhnkzgjq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gintlnfwh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gcehywxsq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gyqhufufx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gnsemdhvh.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gdidnjrjr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gryvyeiwg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnlubayby.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gnrxxweuo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwrftxjew.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gextjnfni.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gjicvrjkw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/guyrbckvt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gftokavbx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gmyxaqrce.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gdfuxajfk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gvoxdrrgu.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmmbajuud.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gnofkgtvk.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gkokkojmn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gjuuynyuu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gsaltyoca.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gmsyktltp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gsqlvjzpb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/ghrecublp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gqkptxywu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gntoalinj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gxodxcbew.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gdkjucbpn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/ghkmzomlt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gviypokbh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/ghcfzqwig.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gdaspppbu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/glmxbhxue.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gtqxbuexe.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gxcmcuuab.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gtlujczhk.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/greomyqkc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/grhfeftaz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gnrkzekoy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gamgcdrve.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/goveuuwck.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gjawvfetf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gsawhaldt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gzhlfikxo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gchuvxwsc.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gxdgrison.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gbicdiphz.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gqrdlxijs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwyratxok.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnzjtwbxx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/giktqmhht.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gxbqvykqw.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gonzetxfl.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqhpddxnz.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gcfbquxkp.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/geklijgek.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/grxewdakh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gblhlijwi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gegnqrjsz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gwhndcoxj.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbvshcnjm.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gmvdrjmfk.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gfgyoijzy.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gjqbhrrlu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gtmgsqkuv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gamzspdui.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gcyrxnlgs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gaizdbmof.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gymczpany.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gnylenotj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/guwymdmnr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gicjctfah.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gyjbqjvrq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gvwrybbfk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gxkqmxavv.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gjmszurmp.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gfawnumhv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gyrqivwsw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gdfujnklf.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gsxnuwuow.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gaejdzzqs.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/gccmdjjom.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gawbbtozh.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gjzwpgksy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gdgehcttc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gjlsolcqn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gkqtwebss.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gutrmxzni.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbsebdoxs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gnnwetdhq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gxhyhijei.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwsjqnmne.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gffcfnwof.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzeaqrwvm.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqadgcyrc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gpqhmdzyx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyrjaudgb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/ggpvtgpgg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbuofkimc.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gcrenichp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gihxikewn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gwodjceqq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfciiavqz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggcheeefr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gtaqpzmgd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gsxymmuys.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/ghdzbqtuk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gulvohiqc.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gxttimtzc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gqrobkgui.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/grhebmpcr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gqqzwluih.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gbbeivfsi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gbotujovz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gxnrojkdr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gipcntscc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/ghtrpinga.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grszowwdu.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gsmmmadai.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzuqcmhdh.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gsewyemad.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gkuhrpowz.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gnkhqoadv.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/guvcjkygq.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/ghkjofbnb.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gyqjfhohv.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gsxwfjfjr.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gouzufjhl.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gpzptcueu.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/graswgczw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gjsyrmcsc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/guuttagej.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gzsghutxj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gdgicqyej.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gowsayvuh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/goskfmkwy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gjbozjhwd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gadtxebbj.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gnocgztfj.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gmsdcehkk.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gybkfuqgf.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gkyggfqbg.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/guqflchfo.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gmiyjxgyz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/grauenfxs.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gqtoaikpl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gllnufgan.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gpqxfpryc.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gmzbfypzj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/ghmjiexvm.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gqahnghfo.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/ghaigoxwg.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gzbycchuo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gvxvxtxqo.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/glrmqukwk.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/goamxcwbs.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gawiabnfv.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gegvlyjoh.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gogkvpkas.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/givzulepe.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gkrofystv.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gksekmpci.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gvuzdgfzu.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gagwmykrn.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gzooytlpk.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gaozsntmz.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/goxfpspyk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gtdnntofc.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/ggejfkptj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/golffudao.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gvoswnyvz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gqjgdnwjf.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gfsqfncda.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gsbkkvftz.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gttrtlqlx.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gqssvzhge.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gfhngrfcb.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gjjauiekp.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/glvqnezjo.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gaxvrvruq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gnxwkxyey.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gvxontdxg.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gpcchysbm.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gbufmnbco.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gyatvvxvd.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gzmazhseo.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/gtvbffpux.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gzwyxwodl.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gajxpbxoj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gqmvqitzf.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/ghnxoauol.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/giizbdxak.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/glekhejsl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gverfbeux.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gsnkbiram.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gqlglzfxv.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/glkeaecre.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gdqefkpef.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gqvnmwvfp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gfwkzicpu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gnccxxyny.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gbkujsexs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gofrhdfkc.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gcbnoqakh.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gsdvtqfrn.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gobddbyzm.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gjcwvxdho.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gupppxyvt.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/glwwiodnd.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gbptlraug.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gapueaygk.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/ggukhdjqy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gjwekzljf.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gtghgktjc.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gkiksqhtl.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzgkarqso.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gtychshlc.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gsxnadkpo.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/glwstahlg.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gjkhpyrfa.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/ghgaedoqj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gphewgexm.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/guwkhpzkf.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gmnhkdkti.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gawzpjcsz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/glhwfkrki.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/ghrzbkxut.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gzogfeopa.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gltfhckhy.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/guiumanpy.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gftprmghn.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gjcclfeac.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gkwhxrpsb.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gsghtcdfw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/gmajmiycq.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gkatfbnkp.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gywiraqep.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gmfvejrte.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/ganonivfx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gsppirqiv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/ghbysewwm.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gnagewdni.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gslycoyay.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gvllntglx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gebgydklq.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gonokqxsz.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gpvazysso.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gcjayhvvn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/giihzbxnw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gmmkxpwes.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gaqcwefcz.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gdqfhtntp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gsfukowlw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gnllifonb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gmmgzvfbc.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gwxcdaqwp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gfitwppfr.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gfoelxirg.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gyzrhdzyo.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gyqlyjyyg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gneupmsfg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/grjqqvhjg.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gdfukrfom.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gtgjlvona.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbfmomggl.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gjsuqpvbo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gekfbqlxs.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gkgnpfsvn.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/guatcjqyr.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/goanapyam.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gjuvmxgqh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gbjtybbkp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gvftrihqm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gcgzvytqz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gyxhewobx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gtplszben.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gerdcudwq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/geawfbzhu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gbigzmmnb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gfxngafmi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gqstsclpk.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gwsfnlcja.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gpxllegov.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gzzsbdwcg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gonurorhj.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/gspswktrn.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gjlsdehxv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gjazqugbv.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gzziuwuxb.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gkecvrqbw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gbpqmtiog.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/glgdgrvmp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gmxrfeysp.sHtML


<!-- 参考信息 -->