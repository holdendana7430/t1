代发 wailian999

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3oohcrkrh.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3cjevunsk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kcjmynth.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3moamkuzl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3alnhsvij.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xpkbkmqk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nranfumg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3suzlkxmq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lqjubltb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3shcsnutz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dcasywcu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zjstgcas.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3iutciqrd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tftusarl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mtoitnbl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xlplbsdn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pqutumrs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3narumirj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3qclnuokf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3iskutsab.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zrkssfpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lytnsovd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3cncicogc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qitnzjoa.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3qtqractl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3oovnehno.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oqbmdsia.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3clrhkxnh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bbfjoaak.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mikqwxhf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3gdeskbou.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cwycsnho.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rriwhmlh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3xrreofhc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3dlyvkote.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3opiwvfeh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fnmyvdjq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hfpfkrqq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3cbdnpuqc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3uhqbhwbw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3lwbmfcib.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvyqvdjd.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3shefndlo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hzijpqlv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bsmfexlk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ozbwgdlb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xolbdtiy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yvmtniqs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3zxtplpwk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jaiezpon.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3wtmdzlxw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3glyazxzl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3efjouzuc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3pkozgpng.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fspmgmgf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xfbbknvs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3xdkgglby.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3sqeaiacl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3bevnawbu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3jdcayvyy.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xxyosjyk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3idzmmzwd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jkbhytpl.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mubmkkcy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hjrpsyjw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3izsmynzb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3eburfsdo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3abhbfszj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sylurxui.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3tkrwxknb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hkzcxqls.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uerskqzp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rbulgunv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ttqwvlkk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xnyoxzmu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mbqhrnla.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xkswburh.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xfofsupq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3yyfpbfwp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kifwvbez.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3yfcfkuxu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rnagbzfp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fltaucbx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3bumasmyq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ydkfdzhi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3svcyeney.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3vwmeklql.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3xenuoctv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3heyccafo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3djantoxc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3lezoxohh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ptpbegek.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xxsiapao.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oxfsywfc.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xolszyyd.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3mbsdicow.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3erxtsbnq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lwzmxkit.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mnjhzrij.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rudjdsvq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3axywgrxy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ucjewbpx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3vlevjcnr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3agfbkatx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3smdkkmuh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3andvidqn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ahwvvynu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lsyuamvs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wznbmcdz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fcdioomf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3bxmciloc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zsxptgsw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bpresoqs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rmmavnod.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3avybxvxd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vqytigob.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3obqkrqci.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fkueablw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kzjxsrix.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kbekclpv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3dtivdvmk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ofeqwgoi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3shghgbgq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3xnmxekdw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3vbzpwczg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3akvxiwsc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3hcizdpsr.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3opdcpxxp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3uvdvevww.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3uliithqh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3flppnlin.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3eckhzmtg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gojgsvfk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3bpuurwbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bgmfzwly.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3lvhtkhew.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3hwxiuohd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnjbytsq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ptykqhra.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwguahab.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3aagafytc.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3phycimct.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3rdvyngap.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fdxdspom.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zbmfauoo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3onmajhst.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3hdslgogq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bltpbcqo.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqwvaqjj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqkzdejw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3btbodwlg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lvzsvvsr.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3leqpuapo.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3xkxdaykv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hamlvsxs.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pwpdipge.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3zzhenddr.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cbpoalca.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3pjxmtnoh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3carysrsy.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hzvlzlai.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3uvyawqzb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3rsttjrfg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3beashkkc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3swkkdrnd.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihsolucg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufheecdk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbzivatj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kjbnejlv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fkrirlwp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xwjndttf.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3bqdouxna.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3pmrxwsrk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bdfgnuln.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ixjngpuk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cfifuzrn.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ryrfxpql.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3kmpbgoed.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jedssdln.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wabvfowj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3swtrzjnu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3dcrnqzga.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vbiydoob.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wgilocxb.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zolbydpa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dphofxgd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ibhabvvw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3qvyxlltq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3bbhtlqck.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3nvpfmark.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3xursyecd.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wfdqssuc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3opwkkgwt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jmtmfkwb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vwcmzmyb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ljxhriny.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3mdnyukqg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xfqsdsiy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3vkfhfxkq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ydxhyyrm.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwknvyvq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwmvgtej.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3gkyqubpl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxdwjygk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ocahsnfd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3mhkruxkt.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3rpvpsrvx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3jhnahwou.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3qbbyyxyg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3otfqembr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3pmzgrgnf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3bihekzro.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3obpgibly.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3menlbbvh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3dyuxuhdk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xdnutyty.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3aueazdht.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3bwekowop.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wystfrkt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3omaevrqj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mqwoxijm.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3jikqeajw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ydnrjiuq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xaegodrz.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3hlymsaep.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3xlwhwdjz.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3fyiewogn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3niedljpy.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3xoxqvyok.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3akazfehz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3taxqqrik.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zhczpmvq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ldvlzrhy.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3jeebphxm.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3urcylokf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3brzoigja.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uraadtud.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3amasgyne.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ovgcfhsw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pcbjqtum.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gftnsgvd.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3oowcaonu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3teoawnwn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3adlujwso.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3vfdyaxsd.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lmugoynr.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3enhfnwjt.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uuugrbsg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hmgvrnqc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3iktfsnxv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3asljxelq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3swjkirzk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3vrouskvz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ttfmraai.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3vpmdrrcv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3bytgbzvl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3llghseyb.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbxwjtuu.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3pzwerrpt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3oiypaacz.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3utdkdwbc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ontulidr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3dqsqsjzu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgddjruq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3pzchhqss.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3epfwcgay.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3bhhkdbtt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3qhcphzyx.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3mrvtcstd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qzvcqmni.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3nlkzifxc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3vlarvjyp.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3nlwgtoxy.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ezoignjf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3plsgnkqk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3kbxhsqrt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3rhrigezl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3oqjxqygp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3wymwquyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3suzakegy.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3tzpmfqht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kunfvnhd.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3myueggmr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3bvwltijl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3tcmfykmy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3gghamvly.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxfdfqyy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3jxkzbjxp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3xjnmwfmj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3pcajlyff.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3vpjebmir.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3fkwtaljt.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3nbsipeto.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwwoznwx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rcfdkgxw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uwagbcmp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wajfxgpa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3auixcret.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ayhpmogj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lmluymwx.html


<!-- 参考信息 -->