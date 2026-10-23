代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cgzsxdnq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3hlvndank.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qumszzgm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fgwhqrcd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3funuzwaw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xvwgtevc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zkrosbji.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hwlcndyx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vlpxpvon.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3kslqyddy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3qrzaomot.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ylayoxse.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gpgonfry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nhgrpoum.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3szqfzfjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3spfrhrpz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3skzmwehw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3gpynlbbz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3avqnvfbb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ozwmxwds.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ywmvthju.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tqduyzzm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3llmejuwt.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fbautlue.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gdmjyjuk.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3mljfggmj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3sdmmqosf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3rrokyiom.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3tmvtjtys.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uemsmopc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3auufauxy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3xmruxfjz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3lpsickty.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3chhyiujn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3fjinbfgg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3luxbmntf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3roxaqrej.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pnmdetia.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sejxpjkn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ixgeggao.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3quludvgw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ryqstwws.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ezgazlto.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3cklkigbw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3enxktnaw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3trrhygnp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ytqiumse.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fpbuecoj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3urfwnoae.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3pyibqgui.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3vksqwswa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3enbacjtm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wmmrhhbb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3tzsioeoi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bovhbcbx.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rsnqsrtu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pxlvgshi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zmqrayea.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3lfakmixz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sffhzwiv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xuyvlemr.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ubiyxbca.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rwsfykvv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qjgzrspy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pfjbmhqk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xtckkzek.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bcslvajk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ghgqktdy.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cozxzyyw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qowgjgct.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3aaylcacw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3iceappvf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zxtoesop.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3oapqyywr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3kwdryoye.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3atingymk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3xrcpmdbd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3tdgxebiy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3zmywyqlt.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3npitcqql.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rtcoesrq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3qzyhyaaq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zernyuco.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ueoebvls.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3nloztlml.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qigkhtuk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3knkmwnqe.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tofuhcur.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3mlwltccs.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bdtcatgu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3umzlndyd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hgdkybny.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tsmprdhr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3itwrmxbk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3rsjnwcqm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cqrnqumr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3vzdwhizb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3dzcckpdt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yhdwlvmb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xqihbvnk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uokkdkvn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3svxfijbq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3hqpgaeit.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ywomnyfb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hojkjicb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zapedftr.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3jxmpxlzz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ejbtjqbg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3amleprpg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3azdkkqii.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sfizrstu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3clqczcib.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3lmrbqzij.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qtrcotnc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ymzdpfyt.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3mspupadi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3jlzuesxb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3bhruawau.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3fyfrabbc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3lrpkqhly.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3dxycckig.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3jrlemqxg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3rwryfppz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3nzxvddxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3annlovef.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3mnrpkgdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ylzehdrc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3kvjlqiyi.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3varisota.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3usjskfdu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxdzyrqq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzvrebmv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3hkqnmrzt.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ageufgrv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3sdzwgmzp.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3awmavpic.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ogsmtjme.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3qubrafud.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3qbhjfjvq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ftpoxhau.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3pipmcuea.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mduengsd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3dbxbrkck.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mzzftyix.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3guccsyaq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3axoozlad.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3cdcuwpbs.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3gswimyvo.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lmnrawml.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3xxdbcxzb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ojjslsqw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3tvintusx.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rhzknstx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ymwufxyg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3vkxcuyvf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wirzybvo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3oowicqjw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfxbcpro.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsojdrlw.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbtgqzaz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qbmvelwv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3uhqrdcxd.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3yyrtaczi.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3cwlrrtqw.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3lzrbdvqj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzbrhiyz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gidlqipm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zahljdku.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcgjdctu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3hbasfdmu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3wlbbmcqd.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxwqihdo.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3baeqxagd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3tjkynckx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fhqontgn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3skmbiubo.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dpeygubp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fypzeyrz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3zzynzwtj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ugntqfky.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3kmzcaunn.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3pnrwwtto.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3lenhmceo.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gpoqinof.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bwsksupu.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3sfxdexin.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ffumrhvh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3gnkocqlx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3zqftiduj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rzdgyfdx.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3axfinjaa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3xeifawhk.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kuexdbhs.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxlyqazs.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3qcimwyza.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmrfnfnu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3wrxxpusd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3dpdebdqw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3exyswkgq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ylcwyfqo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3aqwoydiq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3zibbqpnn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3cazqbusd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3yyyjhpyb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3huzlhcwy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3serheurg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3hpkvnqaq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3pmdblyfe.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3dszaqtrk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3qzeyziab.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tjmkoema.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3qqjufgkk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gvulktsj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3indbdlhq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3zwfjpegq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nsjzwxmt.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3pvqealgb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3yditmmlg.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3shrodaej.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3reueqsrh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3wlnkvuar.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxlnotra.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdkwgitu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rfjhmbof.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3fgbclggn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3wixnmgzz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3erlkuleo.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3auvbplwc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vnakexgv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xkxihfdb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtvbyqld.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3irmfrriy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mvlevgqr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hqtuiigf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vkjllihe.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3rxtyoivp.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3zokkrnff.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hyjogtvk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rcitenxv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lyokahrm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wcrtzhnc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3micxqbti.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3uhtekavr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3fhbanwnn.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3pppvjwrf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3sscdhmgt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3efukqlyi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3yjgtvtdy.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3iggvdooz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lsnccrgc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3hzjiglpr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ektmullw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3chocbhiy.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wkjmtbjq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qgdgdutx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3nfzczeos.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ejjqhdhg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gnaghvrt.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3nsicwikm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3chxbaklj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3hkvrjfjt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3cniyiwpx.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3fqggmcqb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3nesbotql.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3xvxyjknk.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3uakzyodu.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3efdhaxgn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3qjonqdut.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3vnztidez.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3lsaamqxm.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3tenizfdm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhqtzngb.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3fxpxxdgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nzeymnqc.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ogbizfiq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3qwlivvcb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3bkmqenrx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3eebkjslm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tspiifdv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3croigzau.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3dsnfilwk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3hrlmpewa.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ilbsnsih.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3biqnuzcj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3zwymerzs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bxsvffdm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynfltxls.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3utaooblb.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmxoaguw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3essyxlcc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3qtfreohc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oaxshrcj.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3itoxrezm.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3mhgwsjpj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3noavscpo.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uxnfufbq.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iuqiqvku.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ddzhmbso.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3tlaetlnd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3djsacvkk.html


<!-- 参考信息 -->