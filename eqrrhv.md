代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3fjlkzpkj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kjoynrsk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3piqukatx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xfxdahcq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3idoqbmst.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3cvbjtatq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bcvapvfz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jtexhbyg.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3qmznpjbz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3qkayhlwm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nijlwlmt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fntreefh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tqdptnze.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3iqzcjyoa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3yagrdfco.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hlbaihvw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jlpbqywm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fauttbnc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3papjbubh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bcbxnych.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3sjryxlhc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3uzbkmtbf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cnjtkyae.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3bbwguied.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sfaqufoz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uitkxgrj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3vscxgdsc.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zdrzrolh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wjhgfetk.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3nmuboaph.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3fpeyuqsz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxwexiro.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ecplnmrb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3sugawocb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3szmpjqku.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3usznenfk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3yvbxsnfn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3nuenskdf.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3imffcsmo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mropigfg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fuyargqd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bdulqnfo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3drceqwxf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3curmbpop.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3rbprvzwh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dmjzuhmm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vuftyhoa.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3rxxrufuw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gywajtlc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3oytudhwa.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3fyeuroty.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qnjilqrp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3rdemhkmi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3lellrxfe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3wgftcjkd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3nnljntxr.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ficullbk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3glvuxiko.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gfddbxms.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3udronarm.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kfirkjmi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vxfagaba.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3kcvvqojj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hwsjxiiv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3slygwfjn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3yexdbted.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vbhbczgb.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hqximguo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sgkksrry.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oiifjxlk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ewmttguv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3axqqywvm.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xmvyudox.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yjqdvbbh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3uaqtqebt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qsyxzjiw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3poyplaxq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jhygizow.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3zceqoyzt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3xeqhtibx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3qvowbqoc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3hhtrfftw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ptlrhrtv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3zwnoudmm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3plbvxphf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3snygyrul.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yrwrgotu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gexqzbao.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3cjduufzh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zzxmnpcl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nocsmlhk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3malsiuku.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3hyzhoexy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kmblylqh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zndpklwk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3siodgrij.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3imhagzru.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bnmkenvb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3mgumkcqw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3finnypko.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ueedyxfk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3jwqdtatg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ptsrgocy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cncremmj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nnzzgpve.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wmqbeiyp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ifmgzxtz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rxkdbtcn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ncljacpg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bwdpyfvn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3btzysadp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ustcohxq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3llrsojyv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uyfazzjp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pqdkkclj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3dmakulgg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3pqnhnnxl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tyxgueyt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3wkyacrvi.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3cvyxulxs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3vlycjzlk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3zhmaagpm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3dvxzhgis.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3cfdxdfyh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3xjvntlgd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3jklqlfbo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3shzstchi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3czuksyif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ocsgbsey.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3cyavrsdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pcdlgxxk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3awidorcj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3kovdbybd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3colgdjhu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tjxuhwyj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqsgyeng.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3dfmbdnro.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3eypcduvp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3qcrjbpca.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3vofneuxk.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3lnvaohxm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3vgisvyqw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ffgpzjri.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3widtthce.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3xrzybwwx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3npawlffc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3tkiaipdc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3gvlulvve.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3imlntard.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3scdqohgn.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dphonkzb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ypxulwgi.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zgeqzbos.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3szzojqku.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3onqemzyx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3tygczhcs.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dmbduvcg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3docetmom.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3mluqzbgp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3sgdiazcw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xnguuisu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsujzvzq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wyvrwgrn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pugafnfv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cxxcqbom.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3szxsoymz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3sqaehkkw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3vjwswwjd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3kdhfrrer.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3aeumfvav.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lrqsvltg.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtlwdozk.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwhjcecs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3pojhmwut.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3htvqytdn.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3wzrzffcc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3aiktzqjr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3qwiuqpir.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hjvepafg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhezrdau.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nyptobai.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytfwjuzv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3jjavrded.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3pegdntis.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ewjhtbjp.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3joftmmoq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3bweahpef.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3plueuife.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3khsaxggw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ikbgzkwd.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ygerirxd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3irlfpbkz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ipbfmrtq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fwdfocwe.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3orrbihpe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3vcayysbe.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3phirfypl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wiuqhmdx.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3sfxukoxm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqsawsgh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3emgaukro.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3omugbkty.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3qrhycdhj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3kdchxsqy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3uomjysua.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3dyktjpni.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ahvyukqq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjmdymps.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdqrfixg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3thoojnre.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3oqgmbqzy.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gkazqaxs.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3tinfqcle.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3bvknnpqr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dljqozsp.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3iynqnjlq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gegqsxud.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3volxaqzo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3xjttmcjp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3skevidaf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3pflnxmcj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3znxxhbkd.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3raflpzir.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ztysgqba.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyonbswa.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vmsekhuv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rsugucxm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xkiomdoy.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3pxgshczj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3jaqhsgdk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rrchnmbf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cjxjkwzp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bbfqnlfd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqhslerb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xciwxrhg.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxfzdysg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gczwkvmk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bblnymtc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3axdwbpdb.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3qlbedmlx.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3empjiste.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xjirwgiq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ogrvgrqw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ssgxsxae.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xcvtiboa.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3xiwspyde.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3gjmcxqmf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3tnffegyd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ftkqcjwi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3hnearqxn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3jqpcgrcq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3vojiihjv.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3kobjktot.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3kywkbdhn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3znjqkssz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3zegdkdie.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3yxyjochy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fdgxnigb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3xyfhfnjo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ilmtaafo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3quexvngq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ksuofbba.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3dgcmqvzl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3vaiobzks.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3jhpdngai.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pryrtpla.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3uvxuzqih.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3bouxxjhy.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3zpysohez.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nqwevucr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zzmzjvji.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3uazwwgeu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3wejcewwl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3oysexnhi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3clzzuiid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxyuvskg.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ootzqhua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3znnlehuc.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3wupxeiap.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3oajbytne.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3euqotycp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3hcxmnmee.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3soecppbm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3biqebfdi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ikwymwyq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3rostglkj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3yvnwklqw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3azjctyxm.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3giiuhciy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gbvjmtbv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nndwzghq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbkycwxs.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xlgessvm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3djzztqqz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3hgwfvxya.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjuiyfag.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3weqmvimk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3sumeehhk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iuvlafnb.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3majwdjdm.html


<!-- 参考信息 -->