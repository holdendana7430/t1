代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2dhoxwlrg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhfbooop.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2czfgwptw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2termdgga.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2mssgsjwm.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2xgflshvz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2slaijcwt.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2gbimkhwj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2yfihmevx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cxjhspqy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2htxrjgop.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pscolgfx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wahabwde.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2vnehlchh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nagpgnfv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bclmwrbc.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2plvwbklf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mkbybeex.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2unwvmjrk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fuaalahn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2onqjxgoj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2bnkkcmfy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2uvrqkszm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vdqqxjyt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bqgcwsis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sdcrngqo.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2vyoifspv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zpqptofs.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2juruduwk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2rokckwgk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xbcidokc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2gwjfxahf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tsknpztd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nnuftcyc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2nzxvqjam.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qlygrvjc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gtnwwxmp.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2crpegnqq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2pdenjhuw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnoaqkho.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lpwreaoy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rfuxywgz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kglvilbd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2mgdzlzju.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2tvqhfbku.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycrkbwpy.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ofcbtmsl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2qyxihwsg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bshqqacn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2idtsnxiv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2puqhvcef.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2idmvtyyg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ztlhylae.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ppxrtqfe.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mtisbhfn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ucgxqmtp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cqdmyufo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ytbwflmc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hylwmsjr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2nktfxhhw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2zvktqncz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2nbabecyq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2cxysumsj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2qiicebuu.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2blsfbpbk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2yrxqtgts.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fgvtibpo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xgpyxysn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2deuszxey.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wchabjzi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2tdwdflea.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2imobjzkr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2smghggzz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2zqbgtvlj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pndczvmf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bwgrbdod.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cvckgdhv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kwnlguhk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2icmdivod.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2erjyjvre.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2boksrrei.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zejlzdhh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2rhjqvgok.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zbqwvcem.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2cqtrnqnw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2fvffwshx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xnkqiquk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2dkfewcgk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2cygrnoth.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2bonzeupq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2gcmmdklp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2gobinwhu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2fasmtihv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ivxhmkxb.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ckgibgzc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hkqtaqja.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gprigcmo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mczpsiag.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ftslgeft.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sqordkrq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2jzlsbouf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bosvywgd.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vhbnqyha.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qjljddsr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mrgckocd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2oloefpzh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2oytvnbxn.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bvoflvfa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2rguxkkho.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2jyqzrpod.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nqtbvihr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2guvdnrph.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2stwjqbnb.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mqewsplx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2kzuktded.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xpvkqybi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qcvvzrig.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2subewdyo.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2kvxgjrks.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gxixexxf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2psnanbxp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xiifoogo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oppzthlb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kugxmuwd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2sqvvteco.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gdcyzlys.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2tkwdoayg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2fxagxido.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2lvxxmygt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2jlpwlpqa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2smzvishb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lmzuvuip.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2wsreiwmo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2hkssberq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2nuuwaswm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ecbbarvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zevgjkfh.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2jpduqxha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2srcfrhzo.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2cbgikeje.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2dptupefa.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mzjtuckf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjcvypqi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ekpdndfl.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2viimjowh.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2cmpncdlv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2weuadajs.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jkcfbcsx.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2qigqkfxl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2sedrtzee.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqfxkzbq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjmycrnr.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uexzaprn.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ctslixwn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2vtmnhngk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tsqdzyvm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqjokiri.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2lwmhpalw.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rxfvmmsw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qtwypcri.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2miaywetk.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2llauzhoo.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2rpwvxsil.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2gkssiqfi.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hwxcdxrx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2bpeetqgz.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2dreixypt.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mrevdala.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vfrjepbt.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jrbbvqft.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wczrxwld.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2giaxpcrp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2znrooukc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jiyvubsp.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tsjnnsgh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2xqozddfl.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ucgobzwr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uiypvmef.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2iqcehwvx.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewkslgri.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fxshijgb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2dhwjlxcs.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2wzzosdgt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ptrxehvz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2kurektqk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2zybkgdrg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qcelshub.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvbszikc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsppsskx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oscsqcjl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2lsruemez.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2todoaqbt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2sstcqwkv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ttxvxwmd.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2fiynurel.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mtfzrkmc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hhgpqvrx.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dedlpzxv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uvqonvdj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2irmztvxa.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2frldtzqz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2mtstuaak.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ghsgpffq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2gdipzfrb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2npqouqlg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfiumaqc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2xllgngmq.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hizmlzrc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2msbhmjnk.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2yvevtzqr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vuuxmqhm.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2xycikfgw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2hrbtzezy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ozrnzrcq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ptsfgjsd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2gasrgyop.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2hnvkofuy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2vfzmgjum.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2qohalfzy.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pbmxobgp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2spgryijq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2gpdkpwpy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nnpprjbw.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2pkyraxwz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jvidivuf.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2uldvylli.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2thxfgpho.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wcqpebyj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2gibdimmq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2yqixiyhy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2iinxotfj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2musxgtwo.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xywcgzgf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gjxyutkr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdmbkahq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cxpgskcp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2skgdruny.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwswdcec.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2osmbxear.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rbcvivzh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gwsffmsc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqluvpdz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jevljano.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eerkjcwf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2snanbxwj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ptznuxmy.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gcolgzyd.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2zzdskhix.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ahqobgee.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vuqmnapj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kvmfgswh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ynvqyeax.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uaccecyv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2yutdaqqx.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2uqgfpbhu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2xvkcpidm.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2vswenuco.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ywbrxtko.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ulimitcq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2lagniswk.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ujhrjyhj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ofzdemvb.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2lndzvxan.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ubcxvmxc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2huuctyxy.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2fsziuetz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wqirzvrn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cueehdam.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2hxkngggv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2molembil.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2fpcbxuvi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ouycxrot.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2bvsafkho.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gycjqwyf.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2luqaqquw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2dalmzkuj.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2quiczaml.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2nmbrgelz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2cbdkemle.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2hgodivqw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2fgxoixub.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2skelwlbg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2hlviggwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rprqljtv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2noqjlsju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hjsyazsx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2qqposfav.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2cbkwfhdn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ldzyppmw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qmrpxjdh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bshkdvte.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvvnyamy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2phtytjet.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2kibepkgk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkmgpwai.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ichniswp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2sjhrriol.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2erduffwe.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2gsrtwmns.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pysulkpn.html


<!-- 参考信息 -->