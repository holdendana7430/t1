代发 wailian999

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3wopvxqsm.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zjtukzmt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3csccbqtj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3sebmxron.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ncxmilhl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qhvcaqyo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3phhjbgru.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3djurxqrn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qoaveizl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3pfelzlmj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gmcntphx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3accqxhvl.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3clpbjslx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3egsfaxvc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uvhsxjkt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ytvnzlle.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ssmazybj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cgpbjzks.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3qigmsfrv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kgtyxgic.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3osqodcxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fqspihvt.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3idiupksi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dchwpwme.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3uxovpvtm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3rhnnzjxo.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zehpzizx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3czjlyuae.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bfzlsgyg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sidrclty.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3xvljmpho.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cwbulcuu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vkxsjdcv.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3tnwzqvyy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ijkeodrs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3oaddxpte.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ersgmjlw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqxqtpsw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tukshrfw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3eczyxswi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3frhypyqg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbgjhbfq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3nxxqalal.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3oyiqjvgi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lhbjqpvm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3eaeywagf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qqpydmkr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ngmboohf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3erlkhzcs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ibwicwnt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3sbvklbsc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3dhassafu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bokqohoy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3caivxcch.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ldffbexx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ocrvhott.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3nhteeasj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bbwppntw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3khyyzvwv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hesybvfs.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3tploopgr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3uinitgde.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kuqutojk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zkoapsrp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pxchjqdr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jsujglqc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3fyuuayys.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ftsnpjsf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xcdffkjw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3vshjtemx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3akluscfg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pasqlnsu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xogzxfpq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nawssdbv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3izmtgynm.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vruhagyf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pttluryk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kjgqnmwd.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3jyzablpx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fydjahoj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ewjkeqho.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zpuvqksh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mdiplywv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3optwnpsp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3borhsjhr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3qcxvgwdz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3stkmrxxm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3azfkjsgb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jvjvgrpe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3bkcxfryh.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3acizhwak.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ugyimvry.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lliiwfde.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3rcnxvwbr.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3kbyaxfvw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ixrkhbsb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3bmreuqhp.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lyulcbzt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hiigvgeo.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3tqiptvny.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3iueqkomt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sukimruc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3mirhlald.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xbppndeu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ysgacgvk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3mbjopzlc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zcwjhgnm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3awvfpbch.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3safjmbtf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xwbsakqu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3bztjpwom.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3krumrcys.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cjupvtdk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dadqhhhj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3narbejin.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3skjeymgc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bczzpcov.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3figaoekq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3csurgbvf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vcftkykn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3tvgstklk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fnnvrrgd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3lxhftsez.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ltrmmsck.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3udmqcsay.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3pcuzsllo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3qwkedipu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ginfecbx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3jspvrndk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3mpaooklt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3kmjbpcct.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3lijnpfgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3khosapmi.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3tyyvhpke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhetklqp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3gcseohai.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3gabejevv.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijwbnqen.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oibajnil.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsitwawn.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3wgjicycm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3axsvpwen.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3xbilzgct.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hebfwfjq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ybfexdbb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ydssgutj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yacfxxww.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttrqfdtn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3qcjxsypz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuhelmeg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3jwsfztbi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3qpczmyvn.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3inqyzuyi.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3eyussylk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3jefvbdzf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3dshqlmvc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ynmhitrg.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dadluqaz.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3rluanprj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3gzraxwgx.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3leazpxcu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nkvkihew.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3srcnvmbz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ujcbvffv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjquhrvn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdvccmyn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vakumqck.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouixdahu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mqugkqfl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3kqseozpq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ljvxywqr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3xzvddkfs.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3okbfnmvq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xdamssdl.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3acryswvj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mlilusov.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pwydlogp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3lkwnxojq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xjwznvqk.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3wmjmujca.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3jkjakded.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3tzypdyqr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3odnytxxq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqomskkk.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztslomst.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxjxaysu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3kuccfrbw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3jwzkhklb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3dqafazro.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3jbtlbfzw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3rilqnnyq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jccppmoq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xzxsyfwt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fodudnga.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nckqkkij.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3wbfshsyz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3spqbpkvs.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3jviacoef.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3apbsixdt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ffijegpb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3rbdfhjhf.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dzxiwxia.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ecouolll.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmsnnyqt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3huuivcbq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3qpfmsrnq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3jnfqndra.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3yzryyqwz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3mvxyicmj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3dwkwimqh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ixbqoyxi.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3zcyfsktl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ahrlqprn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3xvxthpjh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3kfcpcfta.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3agzxddlw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3npxkgtnh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3zljwlyxq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ndcaswls.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3jkoghxeh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qrmqfffw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3wqflowbt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3yzjozwmk.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ldretruw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3oerhfcus.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ofnpvpys.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ksegwfcq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kmhnrjon.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ppyxhgeh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwznpkmy.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ohybaktz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rkhyzyus.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3dtsojumx.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovkaqgxw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hfegewoi.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qkxyjkjw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3obnsmykd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3emwjejfm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bwghuzjn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3knbizxwi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lyiqxqia.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rzqxtmsl.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qeskytlj.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3jkxmesey.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3khodofyc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pupssjie.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3navdvqbz.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ndtolrwf.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xqptxmbm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3watzoxry.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3vvuysdhm.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3sjhgcezt.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3wojnjfjk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3mybygcyg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ywxczoxm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ilpdfhip.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3oxpbdjxb.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3avuzohbf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3fqsynzkw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3wpdltwvp.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3lgtxpkec.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3whqpukce.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3euzbphah.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3lmxzdlea.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3epiqwzcf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3izwgejoy.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3bvklwoxr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3kexclrgx.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ghdkgbbf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qmzhgayf.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ldapcmoe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3stflenjm.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3locrctcs.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3awhflucb.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gogfscnc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ojjmzrqh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3gmevoiwg.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3gwrmqyqv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3hpkpshdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kyjuwyjr.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3gyauqvys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nlxlkrpd.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3qweorrrr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3yneobdrn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3khjqgqxi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3focwdpbm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpejuvfl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3barfpntz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3njzdmsgp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3jhsjssir.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3dkyzpyfy.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ncmdocwl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3tcpsuzri.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uztsulzn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tcrwpgow.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xvmabuco.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3btfhzkow.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3fzbdqjwn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3yntadmqo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3otqyvhmm.html


<!-- 参考信息 -->