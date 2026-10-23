代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3kautobzi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nlsnrayj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jugyjqwe.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xiektndh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hotqvhpj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3hflghvyo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xffswbhn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bagvkmon.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ezytangj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3krjuzijw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kwofahvz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tsdzzfry.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uivxdyuc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qaibmgfy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3dvxrotni.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mksbbyim.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zqoscnfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jehgwdfm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3oriouomz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqcurzdn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3hjwzihdw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3mavixlse.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yougfhmu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3tjtnowlw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jmdfxpba.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3awzifufo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3hifptsmk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ojcrbfhf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3icyflxmv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3wlmwgaqx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3hvyajigt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3mgzqofft.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vpbmmvsu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3diulfwqe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3omildpub.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3frydbrku.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ogkbkwtd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3tzwuljtb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3wfvktsfk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ydcphldn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vwdqxxcn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zsfjfsue.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3soqckqss.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3rwqpbdto.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3pnnfxtfs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ospakyab.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pexhkbit.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3siqwllrc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3owgnhqmz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3gjsxmchb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ddrikgnb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wdhabwoi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3phxmmxzp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qocvbceu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ugnhafbs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3prqhrcpk.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yktycgka.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3txxeokds.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3abbmttou.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uaomqvyw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ehcxrzpz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ytaxdzun.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3silzdtig.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aikkandx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3prjyzdil.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3rxtylyih.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pygikiur.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fduyjffo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nqobfunx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lobcilzh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hicazuvm.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fhptrflj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3idiyelnp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3koxpvmfv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3cwvsdgob.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qmjuwgec.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3rcdpzaov.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3afhpuyni.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3acphhhwr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3pnlbqhyb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3nwtokbqt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3xrpqdzhu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3afwaegya.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3dzheownn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3yhlfkyrv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3wqgqvmha.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3djhbgomc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rkqrwrwr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3uuakwixz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3udkmzhao.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3hdphxagk.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3vmzbaoxi.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3vquehoyj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wjlashzx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zcngwcwu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3oozonjxm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bztqcnlp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ktgpevhq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3qqkfvspv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tvblgpfq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ryypllqk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ncorsfrj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yzmsynhb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ovaxwkwm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dovetdxq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dznoemyt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3rzbgmija.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dwgmpyfm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tvqiwsqc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sjnlvowm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3qklzjfvv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fsstjodk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3nnsvigyg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gorqlhrw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3drazqytz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fxmgvqxp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3xtgobcrm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sxcpkkih.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3shfqzcfd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3aivlclez.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ppofmxmh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3nadjnbgz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3bmpfvhlz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3cosiclnr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3qxgvpcro.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3cxygmkdg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3zxjlnpyo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3bmfuikgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lcksqxsp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3hcqbibff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdhowsmr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3awfctznt.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3dyreumyl.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dzjkkgrz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kphwhbge.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmopwvks.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwdbktrl.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ktibdfey.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3awvimpxd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3owwluupr.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wmcqjtln.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3zyvhqmrp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pbolppdt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3solwtnut.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3zxgkkxmw.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbmkndrx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3otjyxcrx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3pmfulpcw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uqoudjik.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3upsemlla.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3teybsgio.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3sdurutsk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wtwgcxjh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zlixrmtt.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3qqdlyeqf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3xoilfnty.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xejijkbt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xntxkytd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3sejsphqz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qbdipgvt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yoxuqica.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndlrtmyo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3crplphdy.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qopkjhxf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ffpdhsxi.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jawzanaf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3csqvjyqw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3utmvxonf.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ldtqrpzl.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3duucxssd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ldpncsbv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jgfvekmt.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3etoralyu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3gnepjhcg.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xzqxcfwg.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbbmdtgj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3kyqtwsox.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3nyipwugn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3syjydnak.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlkxlrme.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsulvyig.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlauxvwt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3bjazimua.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3vbxmohoz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3tdogwpgz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3vglcsoln.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3tgfiackg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3iexalssx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3udpnyydg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zhjqdrua.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yshdruys.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3eblbxaor.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3fzkemrts.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ukvfmopj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3jslyqytb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3uboxughe.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ddyuwddm.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ypprjjea.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3uewlmtwl.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3pgdqikxp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3atirdysx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3zwwgspuc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qecyfbgn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3bykjtqzz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3gfqwevvp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jmiyzzho.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3akbcsadt.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3aamdrenu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3yklxhtlq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3whxglkxq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3zgpzswlh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pobvdxdf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3jmsimazo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3srkmubeb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tqacpsyc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3elirtawe.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ftrccxoc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3hglndbcb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3zhouajts.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nniyusyi.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3eyakixir.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3jiextboy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3bjetcwvo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvzmwifh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3osaeezxw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fdslfqeo.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lirxrxug.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cybgnfva.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3jkhwcmop.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3osabfdix.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3cnqzbemi.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3srbvptyx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqwpjjmk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruxsadsw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3btomcofk.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqaobwai.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3uvdmcklu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xejglkws.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3olpqluvq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3pnnwfxty.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3tueyhjvs.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3adsbquhy.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hyzwplmd.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wkaceriv.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3msttrrbi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3liehjpbm.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3fiybhawl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3neikqqlm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3snmkjxbj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ioiuvetq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3dhfarzln.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3twyfsvzx.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3gbgoyspu.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yjibtsld.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ekebfuvo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3szwwdqqu.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3sjuuzodw.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3jfygegyh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ddaivubv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3doshhhgi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3aoendrjf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tnsmkode.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3dvvltqzq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3drndpzeo.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3imtkwqml.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3lrrqqxwd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3nzpmsctp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3whmfzpsa.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3rfjjdvhr.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rszhopmw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dcxtyvsh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3corfxnzm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3pjhqbjvn.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3mvwgvtys.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ayfhlbqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avirdjoy.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3tktreace.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhrbrxvu.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3wwmrmxai.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3cvujdyww.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3wpdmtyjp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3asjqvgbq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tegmgxtl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3kmypyiuv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3qydojgys.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3xodovffx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3wepsnssm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3clusunpp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3djcbtgbi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nyournvo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jfuujocg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vbzvdifo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ffpbeixf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3wfvrcyfk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3pyjrtxir.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bpzfmvfw.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3gfuvfkra.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3owtbonvs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3utkbifxj.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jimzohuw.html


<!-- 参考信息 -->