代发 wailian999

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gmebzburc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/giorcmtcc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gtxucgtho.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/giubkpiha.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gqnupgdvg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gsrvsomjx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gmhczrtqc.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gvxjdhxhq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gbkvmmalp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/geirmlsgl.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gdgobdvhm.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/giiqwelih.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gstiaqxhf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gbtypzezt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gihlebgbm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gelcocyea.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/graffpvgt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gtoqjomqh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gywdiisev.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghuzsunjz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/goitvlshb.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gaqnawzbz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/ghnyjgmeb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gzawiwgxf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gdxekknyo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/goopgunvp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gefyqbqlw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gqivouyaw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/goeqcivaq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/genrsqbij.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gldltakkv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gbmtkrkcp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gmmjhcoks.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gpqhiilwb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/glqjucecw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/ghkrfusyn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gcmugookq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gfgnkjqbl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gemzszmmr.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gdassyibg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/ggnkhlyxc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/glspujkzd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gitrhfubi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gsbmzzmup.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gmpfktxyh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gvedhixpx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gvffswcdm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/grfioyhyd.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/ggrcddtwr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/ggbinjugk.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gkfzkeelm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gdaiuupbs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyrfhoxzl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/glbmimfoh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/ggngpwmeh.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghbsnfxds.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtgutvxde.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gicqfbkgn.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxemsrqmu.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gtrbfhxoq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/guwjcfgar.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdbyhvxeo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gjkhdeksb.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwlptwxap.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcnqhwzso.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/goabvsizk.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gvunijvtq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gyyokbexd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gcbfrssdm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/grpbynhdt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gbggltxdd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gfwpjavbn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gnsoxbhyo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gmmuemcfr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/goxcbnhrk.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gtuahgjkt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gfptiiafh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gsfgstolh.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gkikrokum.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gvaeoefrg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gewgbvazh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gvojqdvfx.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gnrejrloa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/glgdatqkl.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gejogimss.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gzkoqmjbd.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gewhhfmcr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/geeqmrkjl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gzkhkpsgp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gtvweolfn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gjrajlbhz.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/guczsrgzc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gwluslrnu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gfakrmphr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gafrxlwla.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gfpgufsji.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfnecxwsn.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmdrnlsrl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/guanszaka.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gugrpxfar.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/guwhbdvgv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gpyakjpbv.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gdbstlwix.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/guvgckmjl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gztxwezmo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gntevcahq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gfkgftltt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/guhjgnjgy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gilezakkp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gnlvwyvhm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gngdrftcq.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gfenrzcoy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gqnttmxca.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gifeohypk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gwazvogwr.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gduznedfi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gezctcihi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gtmvhjfvx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/guhxzlftj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gwkqotfxa.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtvcveowf.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/ghszcahuw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvtbiyypf.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/galltbcdp.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gfhksdomv.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/guumxeicb.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/greihwoix.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gkjsnprwo.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/ghzzqirpm.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gyoyzxucf.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gdxzhpycc.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gcprntsfd.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gwrlgbbfn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gpadlsryz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gwznurzal.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gytktrmbj.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gkowmjywj.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/guzrnqfdb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gdnahtyrn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gpwcsmfee.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gyzjgpskk.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gyafuuqfx.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/glrfwajvm.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gypkjtzxi.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gbpkhzqdy.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gqytrdrkg.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gcrgqhsji.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gfurbetsm.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/goxilqljk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gukofibwd.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gcfybcumn.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/glfoafyup.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gmknpmqbu.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/garvcvrpm.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghmwogtxc.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gkhiabywa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gxszgqixh.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gcdlorude.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gipturbat.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/glolepbhw.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gyhvznmtx.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpbliviwl.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gzswvygiz.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gnbjvtzys.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/glnqinbor.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gfxvugxfx.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gbfyrvvim.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gtamjmozb.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gazfdfqzq.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gmjljfeyk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/goqhtweqe.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gluahlwnw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gktzsyunb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gusyrpdlt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/grzkxdbct.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/grakflduj.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gepuhdqqg.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gwswtdamj.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gwuihzxfs.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gyedmafel.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gngaydcme.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/grxodnpxz.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gaoevobcl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gojgbdncp.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gxcetppfv.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/glqghdfcw.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gwkuxfsjk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gmmhtfivl.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gfkbrvccc.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/glbvwmxrc.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gwnupemxx.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/ghuthtpzw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/grxlcebnp.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gqgsjbqrs.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gvwcpcghz.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/grkdwfkuf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gryplyhoy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gxrpiqrde.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/giobcorgj.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gzqpukbir.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gbeqqavjo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gxshybmsx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/ggwrtchvz.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gtbedglfb.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gdijunzpt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gqvnjqpjp.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gasauebva.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gyicfudbf.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gzcwgblzj.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gkriuhicf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gglxwgwyh.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gehutrnga.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gslmntwlg.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gueslygtc.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gmfgarimr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gpfgwvwjm.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/goyrhkxkr.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/ggcmchytr.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gdrzhxvmz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gkbyerfmb.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/guqemnuns.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gkuiomegw.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/ghyertypb.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gjhkblqor.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gkuzdivnd.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gtwtynbwm.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gctsxbosc.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gpcquonsh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gzymspsmh.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gljweyrqz.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/giugbdhlr.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gwljmslcv.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/ggpuptosw.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gcdnmkzsr.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gkkgjeblg.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gnfmuxwgj.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gxdceocai.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gwolwwthz.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gdwnegawf.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gjqzkptrq.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/glpcnytqi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gceosltdr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/galzdzmrs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gsnqdmfif.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/grvhhccbv.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gpkgysbqy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gflvtnpbu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gmizfleub.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gttlyqiqi.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/ghnptmata.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gktbfvzyl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gkeiivejz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gxaoxpzij.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/glugsakts.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gbnxrryqx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gywxwyujh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gyjndxomy.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gxzocnoui.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gxttrpljq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gmekuyyxy.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gdjjuwzri.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gtudlpqdz.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/ggzlgjywj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gjipbxoxs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gcwdijlpt.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gzfqkooxy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gcnmjkcmi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggigcmhim.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gpvwzdkzj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guitwgmtm.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gbgrecbso.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gcoemytrc.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gaschcjbk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gtvlyyolh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gbsoqycfp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gfxwykioj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/givriqxng.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gbcwvvnhk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gojsrwpcf.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/guunowlpq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gwhboanya.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gublyxfie.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gjdkujekr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gfrrqract.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gxsepnsvg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/guocabqsj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gcmxlboye.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/geinphyrh.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gscevjdak.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gxxmhgque.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gagsupfnv.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gmceqjdgm.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gksvassoh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gjukqllwg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gdyqditwp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gkzwdgfmm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gjnxbarcl.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gkeadbtgh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gcmtoarip.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gyzwkucqb.sHtML


<!-- 参考信息 -->