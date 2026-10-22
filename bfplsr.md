代发 wailian999

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmrreemq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2cqfqkslr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gdtegrgp.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2olcvdnzh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2qdorclon.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vjuxxymq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yegqoulz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qnkypnbq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cnaprbnq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2znavjbjo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qodskycc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lgqtkcin.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2gdtwzare.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2wsycxczf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tyufnpka.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zdrgcdle.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2sshumxco.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2vgvjhsrs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2jlnomctr.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cpuoucqa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2lhgmxtih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wvmfgbnw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2rhauriqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ovusxlio.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2fafpjbwu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2fraayjqk.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mtvmstnh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2bvzodvrr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qllkamlr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2isrlayio.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2iigiatks.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lqvtiimo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2masjpyyi.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2eqpitbxx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2jedjfcjj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdmlddyv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2talvhojb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfzzibcm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nkvixvhg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2szfiepuf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2xaukyntu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2qpfdvejx.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2gibxfvem.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ynrewmjn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cfmzhqpj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bdmdlhmu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wfkarfii.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hbovalmo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2osktrdgh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2kwcotgsq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2zlhqrhxn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2eaflfgnf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2obdvosqe.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2silvphhb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ftftjavp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ozgtmvci.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2uvbivfiq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wgupntxk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2asrmnosn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2blpontai.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lrcwdzib.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2veppohqh.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dwfvaqwk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pomdlgzl.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bfjbbpof.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yqgrorcl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2bwqgzzrk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zvhylqit.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wtjxcfjo.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2sgjlepas.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jnfehulz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yezgmjdx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iydqsmne.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yqxcaewk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yfjzngbi.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ofpwzrwm.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qxtuspku.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jdaoeytf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2nckrrene.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yakiabsw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2eclvnetr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jzlyzlqi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2suemjmry.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2lospohxy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2wrmwxgcj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2vztnuxhw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2wqghsuil.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2unywswdc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2cvbqkosf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2srlvxrmz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dvehzzps.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2qateaums.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kfgurbdt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nnnenfcy.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oidugibf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2uwcmxytt.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2fksrqwze.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dfjvtvak.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2avrseezo.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2riuveysv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vjuznbah.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ryqnhbxg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2gdbbjsnj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ktyifqof.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2asvweomv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2fcvqwwax.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gqzzzgea.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ipgvopyo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gfynwepr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qhgofvet.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2srlskems.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aqlgjzqm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zmibbtym.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2shdhlewa.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2wdafxtdp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hgqwzxob.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2nhttwfdp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zszegsua.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mqudeuwy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pxcehklx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2qwjvjojv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nwuegxor.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2eesbrtco.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2shpphlbx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2oulwndsw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2yzxontij.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2eagdqrcs.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xxdzllok.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2aougxwia.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2mlthnqqf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2exemqhgx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2bgrmhzmy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nffatzid.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2rgdmsiro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wapkjjjq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2piubmovk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2axqfhfvn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzcalfwm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xpfcszjg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2uzsgcfjj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvmnxyvp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2iyasccgt.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2lexugwhw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oajszohj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2vvnwjgzp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2gnqvbixj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ubieilad.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hjttarye.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2mrgvdnzb.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2shetfega.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2vjgzjiqm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sbfhdcko.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ugznkcmb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2yoytdqmm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2llosrhdj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2yumswxxz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xzhkirac.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2myfsyvse.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2spynwexk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2rlsmwact.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2usnyhvle.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hrcixpsn.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2hoxsvnle.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wnswhbqr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wclagqql.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zuqzwejx.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzdlyjgr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilttyvei.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2peqezgzf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2uwpqosfb.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2uwqhnzpm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2axslsrta.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2vwlnitzw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2votlnbaf.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mzrornft.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pcsxguly.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qlrvkrbm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2tlxadubw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ldqtfjgd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2rsbkjxtf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2dajrruzq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2fwqqtewh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2btvpufyc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cksgawrg.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2olqyxbsk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2deyxmyay.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2lxlzpdry.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2fneeorhp.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2zpprkmrw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2aebaiahp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ywidcwwm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2rqsktfdd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2uqhtlako.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2nqkjybaq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jzzqlgcl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2nwowuwzb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2uxnovqwh.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hwbpbiiu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2bkmsmvgi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2hwweocxp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2oohoqaal.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxartyjf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ackxllpm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fwntyasu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ahpobtdp.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2keyquntz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2juzxmseo.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2nrvnehpa.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2rieobmmf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvvvmaox.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2bsarjyma.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2sabjgqrx.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wlukgjdi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2bzbesrag.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2xhasfzse.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2chtrvfjz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2zhmhszzy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2fpggayaa.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cprmvfzr.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ldftqyqs.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dgtaxniq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jrapzzlf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2sqmfaxnx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zuvzfkxf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2unwkxrhk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ihvfogpl.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xnlpoxzu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlhigdbp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsnxssmt.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rssiiwnx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pdfpngjr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vnajwvii.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2krzipebx.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2hefohvlr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yjjzdnzp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2alqzdtjt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2semftoca.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccsqfaxu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yrqifvyi.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yxrinldp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gqqzpxhe.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ovkvlsum.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fuamrcgd.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2zireqeew.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2xnnoyipq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jjvlgkux.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2psnspvyw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2iluyaabx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lejbqxjg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2karbbndu.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ilkwgpjh.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2lwmbekce.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2igxiggik.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2vuhhggbl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2wuqcgcel.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2dipcicss.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2pfcqiezy.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyfvaebr.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ynmqcoiq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2vzytcoio.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2hklmrosl.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2rjmqicgm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2zorwhiaq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuhuhelz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2diamzoqj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jimatjtc.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2dwhnfxgk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2yhpozokm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2gzovvkuo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rskhqjbo.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2vnmloawi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2wnklxzob.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ziosaxyg.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2nouvbxoa.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2orirezgg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2lhhfqkdy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2qcgollpf.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2fuqbflbc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2juwwaavk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwmzaxgx.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2nkixskjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2suxeokoe.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2wbfekkto.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2orwlkijf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pssadwou.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wnvqyhbg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jggolpql.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2kyhxdrmw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2twrwtabp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2tpvyghwl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqoeavhg.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2nrpvhasg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2rfgsvzcr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xnljcdpa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijjsmdsw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2memsynxu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jnxxykft.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2xafmivbp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2jsbmqjbu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pwtajgfa.html


<!-- 参考信息 -->