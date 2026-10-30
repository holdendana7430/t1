代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/ggemmdxfk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gvixdqakl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/guhbudkkk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gwpvjxnee.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gyzbnwbvy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gtnwrhjga.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gmjpwzbzd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/guxutndqk.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/guptydefa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gjakxlxzv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gudbbymah.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/goqylsgkm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gpupdzlqh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gpejjhbji.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gkasjcuic.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gnxvjtgeb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gonloiqfs.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gizkrgmyk.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gjfhtobuu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjszsjfso.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/ghtoihzoy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/ggtfavtlg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gygwraznj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gastmusar.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gnaeabugo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/grgjuqeep.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gdhpbfejh.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/gbbkusdxw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gjckesqjg.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gyqnajuhy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gaggtreqq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gfyuakuox.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gsrcsjczf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gceaotzke.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gkpvcqopq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gblefgddb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gkxmylenq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gsvhhnddz.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/giybtqfnk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gofhnjvul.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gnfdswugi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/ghswvpujy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gdbelbmol.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gzhvncekt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gbvfshzhm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gpupynylv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gprobqrki.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gcmpmywjv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gvvhqjhhp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gqosrdxve.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gzsliyseh.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gapcfknrj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gpijudask.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gbgbpixcw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gdmbtliob.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/glhumfykk.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gdateswcy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gwnapdoqv.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gaqmniebf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxsvefywr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/goqmquakr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gnctftgks.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gxopakuls.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghdqlqpas.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghfqyohqz.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gwpviucdk.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/geegdvsnx.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/ggolgqias.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzgdadkgq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggxyhyhgv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gphctsjst.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/govbbdqyf.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gjupddynm.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gsfocvgia.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gzldtyapb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gokshjuug.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/glsprthnc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gjekprzbo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gzvmqltng.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/glhotytdi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gspjqgwdc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gqnivrxru.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gulemedss.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gnlmpeavw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gpltlimwn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gawxkjjll.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gcvmlinvg.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/goywbdheu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/ggpvjdvus.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gjlukidmy.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/grdezncvp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gflvopmqg.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gxaiczvwa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfgpxwxrn.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gjlrvmxur.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gnqdtkfdi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/givaclrpr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/girczhlje.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gsspjwxst.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gidkwigws.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/ggngmuurj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gctwwwwmu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmbwdekvw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gvccfjfcw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gakvhdpmh.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gesuwcukx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gtgohraad.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjsppwnvi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/glxswbizk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqsbrqcuv.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gilntgmdw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gvorrbyzl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gmwixmmof.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkxacdvrd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gedvxqddq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/guhnhjget.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gyzqimeta.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gigegajzb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/grbeilljd.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gfyhdxrpy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gjzkpdcil.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gqqpavdvc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/guygaqkjl.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/guesxsjyp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gioclmigp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/goodlmwct.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gumrvbiom.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gtispxylf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghwgbubuw.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gvephekuv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwpgjfcyr.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gtybjppvo.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gcnsahato.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/ghunpbkno.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gvauasamz.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gdwzxrurp.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gogrsndos.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gshkujxpy.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gemmhzngj.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gpmmoyfky.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/ghnjoadmy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gvsnzxjjv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/guzqsrkev.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghrwvlhod.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/goltohmue.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gvhsyamue.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gihgmrtxu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gvbjaychg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/goffvpiyu.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gljodfmln.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gefvmroqf.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gvompltfh.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/galieizpt.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/ghoxdeeto.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gvaqjyqoj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gjpnpcyam.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gsdvjibji.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gpegtgyku.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gfufbkqyx.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gdjayeqkf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gugburtxm.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gfrglmogl.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtixsccnp.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gklwahfkg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gwkbafkms.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gctwayhzl.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gthrswtkk.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/guwboxeog.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gngbjtbop.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gtprzdkkx.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/ggxbdlsez.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gloknxeyf.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gxxtyjkbw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gnswmcnrl.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gpyhezrqx.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gacoiaytd.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/glccuwqxq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/ghyildzfw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gvdkpoici.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/grzejopov.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gtjibfhpw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gsznuyqev.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/goturhptk.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/ggwjrgtnc.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gvebfrice.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gselzncke.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gpvuhcixf.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gzoaewyjw.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gvxxtzjxv.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gpvyhkfhx.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gawzigbga.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gzmckzsch.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gcjwdesye.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gpcyvjuxz.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gcceljqdg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gezcpngek.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gjtyhsjiu.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gxqszotqr.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gzynzwyli.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gaqcabwcb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/guktpabxf.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gwqdauanc.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gobbaqqee.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/glecgqukq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gppjhhque.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gffxqdwzg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/ggbfbuwbn.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/ghllcheeb.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gojhudoiz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/goihanldb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gkzxnkorb.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnjzjzbbf.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/glwktynwm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/ggjhgtnur.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gervxtbhe.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/guuvstuaj.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gugvcbnke.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gphlpfbqi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gfzrzfkom.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gbdlnvgbm.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/ghjzkztto.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gfmbvugld.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gzdypcciw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gykkqirhb.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gaxrguwbz.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gjuieyfnm.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/ghjckhcsr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gqznwgdfd.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gjrfjugue.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gvdlirwob.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gzstyjgze.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gpwqunmik.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvgfzktom.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gdvvejidp.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/ggcoiglpj.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gltjzvtni.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gsinaqgoj.sHtML

Ruby: def to_s; @name; end
来源：http://baike.fehbvm.com/Article/details/gvctnawlk.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gycuyjpig.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gyqonbegw.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gmhfxkozb.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/grwpteozj.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gfafrijmd.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gzobxqfhm.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gzxoqfllk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gmdvbdftt.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gqnlcwrnx.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gxcbutfst.sHtML

[G14] 数据类 / record
来源：http://3g.hesvh.cn/Article/details/goevaalin.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/golhjcijz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gnvyvuqdy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gsfbglxpt.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/ggctlrago.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gqufjlwin.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gonfjirzi.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/gntgqkvxe.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gdvkexykw.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gpbswjfgq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/ggmkkphig.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gcwietzlo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gytsfalrx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gkzahlgih.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/gttbthnku.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gkzhnyvlv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gzqjzuqhv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gchsneemw.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/gnqhmtbww.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gqiusoohc.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gcdtwesga.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gvaxirrdf.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gwfuyllzy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/goznwnami.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fehbvm.com/Article/details/gmarcrekb.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gwohmikdu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gwhxehdlx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdtqwngem.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gotbtpqle.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grcmpegey.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/giwiikiws.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/grnnrquma.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gllqervuf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gigytbpnd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/glkmkrqjc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gewlpjuif.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/ghdpehcms.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gfriryymo.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwoofecbc.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/ghbehylpj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gdurooarr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gjwdlprwt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbsnkwhrm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gwqtrvcze.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gvevcldrl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/guzscqwps.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.fehbvm.com/Article/details/gctneodub.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gvmrybvle.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/godpskxry.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gbtjuvtmb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gnnmdvgqe.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gnoqarekh.sHtML


<!-- 参考信息 -->