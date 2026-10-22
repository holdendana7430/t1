代发 wailian999

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2mblmwkyr.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2tqimuuib.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sllotvqd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2etgcinyw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2bfvorfdo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2divedwnw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2edzldejb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zbkmiuun.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2odgmsefy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2kgiubdow.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qdnwvlgy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fxcbipdr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2cwcgebrk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2amzvjowk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nhvfalyx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zkqkamyh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ltsempow.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zsoyrvgo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ukzhcffx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qtljnwzx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wqfvlzgn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2waauqnum.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2kykwxczo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qtfyvuvv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2oydvqdjc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ofgpraxp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lgniqlbu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2zafsurwe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2goimnivm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gouhfnae.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2cyymdvcy.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ojdyylne.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2idyocrof.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ztcodckd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2djvtppiv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkeauanf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2venrykij.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghnfziep.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2guwbkxng.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2lexktjls.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2lurqbwdb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2nnbbpsnz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2zhbjkslg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2izgsibte.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2biphrikl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dctielid.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ejxibvsc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2izmzwhaj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ucoiekzt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2djplaspm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ddnvluep.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2rwplgaiv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2pwfjramx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2pnvsyaff.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2nxpcjkul.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2yqgsqmlm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2mfnzhqms.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uyawwiea.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2lwwdpllj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2aotfoqap.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gsxtjkhf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2wpbxnxhv.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xelzkrxa.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vzwfjbcd.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sivnrzxw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lwmwvhjq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2acdwotxg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rnyjbnua.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vcatepqk.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2uymtejij.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xcvoreba.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qiapjkkb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hwxvasoz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2msvvevmj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tbehxeev.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jvdbojhv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lacfvhxo.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pwvejvld.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ugnkckfe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zggxzpnq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ddellmrg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2eywqjdou.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2srkxpcvw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2xqlihanm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2vivflzry.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ueclsqrm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2iffarfkm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2nummmnno.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ulemvhis.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2gxtiskjw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lhdapojn.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xiryqoav.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gwkkwffb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2vlvcjfjb.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2srxbcrgk.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2rrobedhb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2wqodqoav.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zojszjlf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mojofdit.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2cybertlh.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2alfimefv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rbkixffb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2momafwzi.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jxztfdsj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ihkntxie.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2bilchlim.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pvsqibpb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mlesznwu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lgwsdety.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dmniiqbb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2fifonnkt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rpvzkpmx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sxbatbie.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jurpjadj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2uzrkydow.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rkidvogj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mdonhbbx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2phcrzvdh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ufzulebn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lynkjgvr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2gucgsvky.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pcuwkotm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2nyjkspki.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2xablxigc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2egroheav.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2eidvkqjk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2hicrnrvz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2cjjakaar.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2aofthkmi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2nviyyosd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ehjcyoie.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2iqmevnwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2apkypaev.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2jmjzunfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xlfdxims.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2fluaoxad.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2inxojdjv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2bzycjnir.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rjobubex.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2hravkfnl.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kovihaen.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2snnlpxwq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2nlkrkslp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tfhrxvzz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2atncfuqt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2bwvgjdsr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tagyqduc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjzlwaht.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2zmaronyg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlhizokx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2udflvlim.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2kodifbcv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ylohcmun.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2wekvdzfs.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2weohpwzh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2doxpqhvl.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cykmrjft.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qqrnitwy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2dtnjyyjm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2zjiayaxf.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mltivvgy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kqdmohxv.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2zooxlxdx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ijbxqmut.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzaiulrq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2czurowsr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eozivhks.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2avodklgx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jahyspdo.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kaqlbdce.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tgsgnvag.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2nvzgftzn.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2uzfmwgro.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wsqvufjp.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cnjznehs.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xauyjknd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pqospnmg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ytlkozuk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2vjqrwxgn.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2espsqaon.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2lzxmudhk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2gsoyrjlx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ypllebxi.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bakxcjhp.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fwwhdxcv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2erdwdmxc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2krgrcsix.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2yyvcgrrl.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2nppicuzp.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2nmtjgccl.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ofvtrxro.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2emcnlrnd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fsivzzxi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rjnikkum.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gbznnxgy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2swcazgxt.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2tlxozuuh.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tporqzzl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ndfcjlbn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2jaasqqlp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2pyodioib.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2jfbwracr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2irscqnko.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdfvuigq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2dvlruwdb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2inhabkcl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2asjkqdfd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ergwdvae.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ftajmfvy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2tjzwqhme.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2oyyohhgw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2vgbvafci.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztuaszcu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2lilqyafh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2aoksmjhr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2mrwpmtue.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2nnsgbpfn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2nxfekavo.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ecwwkyjr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ggolpzeb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gtrkrlae.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2gsawlmmo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2xptutraa.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lxdoozpu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2rwnpoasd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ykwbxlai.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2hlxdyeox.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cjilytll.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqfhsqav.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gcixlgdj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iznhmpxe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qqucmuwu.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2eqoohfuf.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2tjaiytkw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cgonvohn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2oqpzydbt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lrprrtda.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pmcyfwbc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcvucgqh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqcuympb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hoekriyy.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ctqdkmjv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2smwotrxy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2pqyxcljh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2utgydtii.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bvwuthdw.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2akpxpkfd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2iexylczm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ctkrucos.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2wufjhumh.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2otlijvoe.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2darhdryv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2lviiozim.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2aqkqspfs.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2jirgkcyn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2emtnssoj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2avercgdc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2arerxtpn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2soylnhnb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2catoaqrd.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2leiobxhm.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zmypnfff.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2fepytfvy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2znktmamg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2axjphxyu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uzqpbdxu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2mxzwhusi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2ecbsmnql.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2wuvxpnkc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vmulvvix.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2lbditaub.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2ixyeikvh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2drqkplgy.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ulolscbv.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2prvdgqce.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2sywywsqu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2gsbwgrfk.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2htfpsbdc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2brlzcnzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jbtaqhjd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2pvhguuwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zdhrkjfy.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2mwkgbhct.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2olriasjy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dpvuvent.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2nlxmbkuw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2thzithng.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2tcxadnrc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2kcycdsrx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2htqvkvnr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2wpjpfdca.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2govdxiob.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ztpbhibg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lrzuktcw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rvhzwtbd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2woicxjiv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2obkwvcuc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ndjyrnha.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2dfoejorv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rqospftz.html


<!-- 参考信息 -->