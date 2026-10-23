代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3xpunhglj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rerdicna.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bamxuzqh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rtzfdmku.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ruwhmpud.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ypeqwpin.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qmdikjgy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xoxtyltl.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3pdxnocbo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3tlhnmnch.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rtzqxuxf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yrlijhdk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3erkpaxrl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cktdyjpt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3cysszshr.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3almywcwl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ayqhahzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rmajlwox.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3uhjsxwlf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qbfigyyb.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3mkdhsgam.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3dknsbwwr.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3khokwsiv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3sasmqpzh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ngleokzv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xrmxerex.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3mgzoxnqc.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zxgdspme.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fhblagsf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3zueaysod.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3jhrrdagq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3gopyghuu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hooihoho.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3evrkprbi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3loyheyyw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3yxswhbce.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ucjbkaxb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3eciroqqb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3pcximgzx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ejjiadoc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3actaxeur.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3agrlrzwg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3egqqeqoi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3rinxtzzp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3sqkvkncl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ayaoodzz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bkbnayac.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3jhvkwogd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3urbhkujy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3frogeidg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gjnpxvii.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wquodziq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3fzwejxko.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hhvylpvf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3tsskryix.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hsbifpkv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tfgulrpx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3avsdsgpf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3djilksue.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3umhzqipa.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ylwtfzrv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ksmwzbwu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3kcoobafv.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mgcqethp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3diwokaim.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3dzpodfsg.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cxzuwtun.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cowelolf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zcufhnif.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oszsyqoc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gfwooqes.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mfpytqwu.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xueghqpv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ldexqubt.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3vmnokuph.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ovlizdkf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dkiyniuu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bomtwbng.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3zdpmgzmc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3rxskxotd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3pjiojiis.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3cpvrlmsr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3rkgmokzx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3rkijopsk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3kytjfmwc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3txbriprn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ylwqnoqs.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3cnsiofyf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3qulbwslf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ajdbpkuj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3patdicza.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3tebrcysx.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3eirxfiqk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hlnzcbas.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iqgijlsm.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3aydircex.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3nxvvxthu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3khfpnofz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3qcqfzusg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rkxjbrfc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3vebgtfex.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3bbaiupch.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fwnkadme.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3khfplzwn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eiirekxa.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nqilxzzk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3kdfkpfok.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uqgxjjvf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kdxzxuqt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mmlzxsdr.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3jsdjdeix.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dpiwkffs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3dkbagzut.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tdnggvsa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gfmizhkd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dlljtqpf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3waxdikst.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sbakehrh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3zbxrcsqj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3oiknhwzj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3brykfzhn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3cwlpubuq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3cytkklhu.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3heiibrcx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3maqziulu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3fbprfmzm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3vlpprrlg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3lyfsnvxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mgczhpbt.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3sddtehzz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3imdkllvv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3bkjfekca.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3qtlgzcrh.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3gjveducf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wzjqaelp.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3xfbuqmdx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3lmnszxjv.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3zgvdpdpb.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ssideels.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvrhqobr.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3yqnbuagu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3irzfzegp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3paibodup.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3czxzwdss.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kihdoadi.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wyqpoksn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3vmgvbkia.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3csnqmpph.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjnsbtpa.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3xhaubjms.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pknlommp.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mhnwddvs.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hkzbepow.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3narmfvqd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3honszzro.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3neodmiou.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3louzzwcr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3yoaycrlf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3bwafgtxt.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wmbfacmw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wjehnnzf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gytqumrw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncbkxost.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wezdlgzi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pydxvykt.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3muvlfzdk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3eyubctmb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3dpcgixno.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ejsuajyu.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3prbvwayk.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3didroeae.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3agaxbmhy.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vvabnhdk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ztumrrvg.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3pybjrfka.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3xdowdftb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3kbqxxcgu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3jwvghnxu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgilnccq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3teyvspux.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3okoqehdh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hinjgyoq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3xrhnceic.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3zzzzgsco.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3jyggyldn.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3qdnpnpnf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3imaizfqm.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sfbtcmpr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wpsjwpxs.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nzgkjyvc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hapxibnl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3mhuacmab.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3fofuftzw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yzsfrkpu.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3kiglatgf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3dzmfpduj.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3xkucniba.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bxgtuckl.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3lvmakcwv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3hcpgycfx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3vtssejhf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ujscquxb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ywpqaehj.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3kmdiggah.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3fotbshsz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3zebevwyk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3kzafctiz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3sagkpcpe.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3gnimshvq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3jldvgcra.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3egxhmrce.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xbqnditr.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3yywwjofv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3zaodxbit.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3andjykue.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3gqnwrzvb.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ckbzhvle.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3xuklqxxt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3njjwwikh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3aiwvmess.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3zscnrzos.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ukiziitw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3pbpglyxf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gngpzthp.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3sepntdha.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjrwaakk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3smpkkzgn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dtrniyiz.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3cwvowffz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3jqoxshgr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3rbmehjeq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3oacuxcni.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3aicqqath.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqshwzmn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fsywjlwv.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdrezlon.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3owveppfp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kicohjsa.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wamqwlea.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3weumhbom.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3hmrjdotx.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nbrylgvl.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jsnfyklm.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bixcfynt.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cgfgsnnp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ubflokwf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3zpiiaqaq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3whiikrrx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3gfoskwsw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3skqzoqks.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3dhffmngg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3cevwsabd.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3jwwhebmz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3kssbpuyq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3opoiswuf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3tglhhlsv.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3aflrzdoe.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3avlhbnsr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3cichjigi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3lyeyvwty.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3tgqcmlwg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xkiijrwp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3pwqxhktz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3bgxoxfpr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3botqcdls.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3evrqurtw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3eihsmjbo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3gutmdciz.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3wplpwree.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gzuffuft.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gdwaklnb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3obbfhvdh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ajywiwnh.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3rxrmqwhl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3wmnzxncu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3npokkqqc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3dmneeonm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zwjgyyhc.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3monzvpta.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3wflmqrqj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ywbapgam.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kezafmam.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zuehlurh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qcctmfck.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3morpkdrw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3lwzyllox.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3autkxypz.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3okcajcmk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3qodsyqeu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ewrxgudw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3txastmdg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gicikfxu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gvhbkxtw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3jwroipen.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3mbessmiu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3otkcmzec.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3xzwtltqs.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3uxykonkf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3afogmibt.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zacrdabz.html


<!-- 参考信息 -->