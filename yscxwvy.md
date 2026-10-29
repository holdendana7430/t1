代发 wailian999

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gepktaeut.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/ghqqklyyy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gbtuidqif.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/glotyiupg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gnxhgurau.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gbvtgzdpt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gokupoucp.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/govlcofyq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gddclmfnw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbthtobil.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gweondlvh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gunkflyrm.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gwejoorgz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gwnwpfiss.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gsyusdait.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gcuelpwtt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gcesogjwz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/grgwhfsmi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gghjbrisb.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvibxwepq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gyzfxcbbz.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gzxnwuqlo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gnqnrravy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/ghzovcevz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gupgcfwra.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqrijpjny.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gihhexmxe.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.hesvh.cn/Article/details/grpdbdmhd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gznqrumws.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/ghzwcvoqa.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gzhytgqyl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gddeqctfj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/giyddoyfn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gclgksrmt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/goxxhlawz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/godlhkhvl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/ghhwrzean.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gkhdesqee.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gagfojmxj.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gttwyetag.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gwkxhjoum.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/grjcxkqvy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gwjlztyqt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gvdbtogcs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/ggjkycdzm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gzdviuvez.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gpivcuibb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gsahmpgvm.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gqenskuau.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/glaaisiqf.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/glyssnqoo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gporeqokq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmlbmzkpp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/glgbkomco.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gbseaackt.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxecrysbn.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gemoxqdef.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gcglnmpyx.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpxdjptki.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gyekajxgi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gwljgweka.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/glhrjndka.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/giwbxoqxl.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/godvtjotu.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfonqttip.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gavplpgln.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gwgqjhknn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gluybpdol.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/getuysayl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gohsxxjgw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gyhovlhtm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gvxskhwry.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/guwrwqqui.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gvgbqilkg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gouneaofu.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gfjruwony.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/guxhpjbph.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gmgqdsufc.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gmigvyxce.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gmilvgiwl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gwcexplxh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/glwjdawnl.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gljijfksc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gewwfvicc.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gbxqrcilk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gnpqqadtn.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gcqygqdqp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gxyzllvny.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gktouwwdr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gpbzjdgqh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gqmapqyvs.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdrmtlpmi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gmazjqppl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gwntwmvha.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtgrwmbbf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gycjxwalg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gctniskoj.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyecckmmj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/grqeompjj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gqhsxfbkx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsdwpxztq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gtvmjxsvz.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gcnefckfr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggmjgxkrn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gubbdskok.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/ggsddmcqh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gxrsugulj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/geduxjexl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gnwtdvvsk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gbtldzwxa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/grjwgqhjp.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gisfghjnd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gaysmmxiz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gfqhxpqmw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gifizbfgt.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gyjyohxvd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gmkdcezxa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gfsimwvot.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gauefhnoo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/grwtibolf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grglfgilr.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gevdmcdok.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwcxzfvel.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/guasmwnnr.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gqampfxhh.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/giaykhynt.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gaifydapp.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gcotxyfzs.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gfljzrrez.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gdthhvqku.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gvhbehpri.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gssulhuhe.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gqjqbwqdv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gxiewbbia.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gqrmzkmmt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gomdwlpop.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gipihjxdt.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gdlhfzvqx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/grwxdlldg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gnlvswraw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/grjtvqwow.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gfkbcxxhn.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gqelamfai.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gynrwfyrn.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gmrfqeyve.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/guzgjgous.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gfrmxcvra.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gsznuxaie.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/ggxvhcewa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gppameahn.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gvllfvbjk.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gwplcxfkx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gxtsobqxm.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gluraufsz.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gimeaaime.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/glpsljoua.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gxenfrafe.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gagnbftgg.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gygqstfkf.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gkbsoggts.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gqyhwhlug.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gztumpufo.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gqgbrnkxz.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gdfrhmdbj.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gktgnobjm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gcleliuot.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gegvjviin.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gavkrwrex.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gentjzyss.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gnptwsgdr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/golnmgmim.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gxtfsrsoq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gyduwujcy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gofsncmgx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/ggzzzprfm.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gilmibjog.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gvbkrfdbk.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gwrkrkqrt.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gektbfaur.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gyghvbkdl.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gzjcmrwmk.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gojtizkvr.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gnseiplck.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/ghxafdvnc.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/grpaphhkc.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gdqebsxua.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gzpzaybtj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/ggkkpdtnc.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gxzhmkxli.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gkfqhcijh.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gumjvmfgu.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gikfvlzeb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gkzqlrgtt.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/grzjdgdqi.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gwpvbgcli.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/ggfgrexsh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gulwfjyul.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gjzxcltwu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/ggtjpqpgi.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gbdjhiwix.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gpspxucti.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gvgutenrk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gghfjolvr.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gimvnfsmv.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gebumithq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gnqznrdwy.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gldzbhvsb.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/grwgcbjzx.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gamxvsudl.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/gnxktrbyy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gebbxhxsb.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gbgqkxawv.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/godkchhoj.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gdoftbnoc.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/glzyjfqhm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/ggntxqajs.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gtahuvkuz.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gxzsxaaus.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gdzwvrmig.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gfkuctwda.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gfmsuxblz.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/guntyvdae.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gvvtujyee.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gexgffetg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gqvapejub.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gybvxoqpe.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/grnruhuao.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gbygpgmcz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gydezmvyw.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gjcdhckhz.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/getuzkrkw.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gxmjmfifn.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gkhtwpnuv.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gtazsziyz.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gstkhxjev.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gaqzkprdw.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gxafsttel.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gnnxrglny.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gtgwufzuz.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gqzlugcxg.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/ghaioderh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gyvmvilnf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/giiueksri.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gwvbihfcu.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gvcgnrfjd.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gmppbldph.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gkwuafeos.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/ghurylwfy.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gvfomxeho.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gvlydvvly.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/guetsdvfi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gvokpqohs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gxjcmihoh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gcuukopnx.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gfcedycmx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gbuugptup.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gthaoqwju.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gnlkyvgpy.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gdprtdsos.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/glepftwjq.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gpgaufiuj.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gavmvjtqe.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/guzjplcbq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gtlobtedv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gcdgdfrly.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/ghgbgzkyd.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gvnskjhms.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnatjdppr.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gcqhpulvo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtvfrrtoj.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gfhpicjwe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gwghqirds.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gqbfoahxm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gptmglrmh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gnkinzhpk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gjtevmcpe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gluzyauto.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gprojkdvu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gxvfalhac.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gbtjroanv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/ggrujxnuh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gkahfedvl.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gvhxiqrso.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gajnbmmnn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gdndrehfs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gjwottakj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/gdzgaksne.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gmgrgiapc.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/geghafafb.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gvypmbjpq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gsilohise.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gzjbjsion.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gqfmnhero.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gmdrnnsjo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.fehbvm.com/Article/details/gxoyanzkd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/grkppdlwd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gueobfhts.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gcvdkamux.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gfdfbnybh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/ghksjwazo.sHtML


<!-- 参考信息 -->