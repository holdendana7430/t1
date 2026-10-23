代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gyqrubmq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3syfijtyu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jmnfdyqg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fnknblwb.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3upilgurk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3haagioso.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ndfokpgz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dxdowalb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lsthpoby.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zljqjuhy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3asjufstn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3itigkysv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ujgcipgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bnwcrvmr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3avmvuktc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lcjlcewg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3adexxmdm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3nyymuahk.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tzglyphr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3pzmallkq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fzkiublc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dxnrvfoq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3bqhntiet.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lttbcycb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fuppnjkm.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3zggnrxam.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3opffjsly.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvrtqfdb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nompyutq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogzmhaba.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tsipzjof.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3heegqhuq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3edomlxyg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3pwddzxdm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3jgtybntp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3gfnycqxj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hcygmhbc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pykmfgbk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ezifduvh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3rroixfmz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3cnikiwdo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ttynvtuv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xyyrsgpc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3zmcciads.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tvfaxonq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3mscnqwgs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3btbxvcrl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3yciwdzow.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3jusewtyo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lvqnkhyc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ratkrplo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3cqlhdhix.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3noknclho.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3spayaesf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mcbzcfjk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qcngjzow.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pehztnqa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mcamcaff.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3coazlhiu.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fcvxdino.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jfjrpucx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3zbmmvjsg.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vqowymsw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3owdpychq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wfqkicfm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mfoyczsx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xzogclno.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gqbxecnq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cjfgwvfx.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3urrpxjnk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3vqdbzvqi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jiixahme.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bwaogiig.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hapsyarz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3uvgtqcbx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3smfowxtr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3afaklwsi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3fvojdgrf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3tzuzgbzt.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3blsqzlht.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3sziikrwe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdsdppkn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3iznvnorn.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3owxioyma.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bmcqjtjb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vrrnavpm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3locprhpd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oiaujshw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ivyrmooc.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3klxwwbuc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hityvrca.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3juzggzjh.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xrjyslxf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bzpkyooe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3idvbbusw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bofxmswv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3xjerlxqj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xvfswuzl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gvudxaap.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gwhflvuz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mfjhaely.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sslkogkf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3thygwkvv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wxanjsnu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3agopuedj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nnuztvpc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3pqaxckzz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qkjnyyzw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3waxolyek.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3eqmrhibb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qtkzhbbv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3erpvsqij.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3lqxojwth.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nvgxqysc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ahjtdvqp.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3kdxddpqv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3mxxtxmfq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3uscjtkpq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3itjmzolg.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3miznegab.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3kqqfleng.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3dmynoxur.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ryfsoqjh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3xscvnybu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mpkrjoon.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3fjxjdonv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3usgudnmu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3hzsyfesw.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3sapvrlnr.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fgxgjcyh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ftxevncy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyhzlnjq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zykuzays.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3xgmikube.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jqlswmwr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3dafftndd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3snrivtjl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ncldsmpk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3bdynqdtb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pfzeyqfy.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3futmrgke.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zbfewpih.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3cfxddfbo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kdgwbtva.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmyhvzzc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3oukbmjkd.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dzqztgco.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3dzstnswf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3sofmbrdt.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3mglvohkh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3npymlukw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3fkzncjey.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ycrpjlco.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ldhdbqtc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ztfreten.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3oxhzcrmv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hxcvgtxl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xthqzics.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cbkxlhdi.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wpabkysn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ihzhcdcf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bgwpusfa.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ygvbuccr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3cqvnfmbk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3lkhuhrkg.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uluvsdnl.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3efeduhvd.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdjmtnoh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkokiwuk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3efzqwlge.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3fqrzaphx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fclhfget.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3spfktspk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ksrilwpy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qqbekmvh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzbxzgbj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzjvneai.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmgnlfiv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ukbvhgvr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3jdtocqey.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3xcjjtgrp.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3iegdzcer.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3nlhoikjh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fevoelas.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hpqizjbk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kjlelcif.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yedqgyrw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3nyaxghfk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3aozeudno.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cjqxyjch.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3qcyunbpg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ubvpelqx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwlofrrm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqfctdet.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3phqkjarl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3idvviywv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3dqtnxlut.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3jvwczmho.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3irtqenov.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3kqhiunwd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3uhvxbtjt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkdogmjv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3pymszizi.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3rylrtwmb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ncuxyqke.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3cygfigsb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3wpnkdrdp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bijzyqlt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3lxythhzu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3trulygfa.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qxksmayq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ysmpmuwk.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ryovpgww.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3cspahisu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3qeumrvct.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kandsuhf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3shhdjmlw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3kelsspmn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3kdgjqvcc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3brtfqipk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngyidgfu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbyjaxcj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3seacjovs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wqmqsiih.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3mlunytam.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejgehbxw.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3dwninmqr.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3eiddvavi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yesgulac.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxvmsloq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykhbdjjv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3molaitlj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ltouvgta.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xfrqjrzu.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rbvrzdvq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3lueixbrw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3kxykmqiv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qkfkalha.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lpwuasgs.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vaybtcmr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bhmyamaa.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3vigzfbow.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3dznipwjh.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3kdvqzoxg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3tkyzkzvg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3plpupoao.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3zzswdtds.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3uqdrdzeh.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3hayyvkzm.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3dibqtqzg.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3tfggnqhr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3vsxrxfgo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3pdlteygy.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3jlyicfeb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ltnlqpcg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3shshefdl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3yzwyftpp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3khpghcku.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3njftlhta.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3iwmutnee.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3cckyojwt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3dnevijrr.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3gtuwfwrb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3nbhqiwbh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3xyjncdex.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jovylurd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rdwklkkr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3sbcpphle.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3hqjithob.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3adbxmcfp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3cajprbxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wmubxfqw.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3nuwfmvix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hbzwctqw.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3cgglebpn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3yngowqzj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3vfnovptn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3lkysckjw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3buwnmwqn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3uisxiydw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3jrnrkjba.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3sufyeswr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3iifhblpl.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3nqrjvqsv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3cbbmlcex.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3grvbahoe.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bniaidfj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3soeilnav.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmdnmvdr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3codchnqt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3mgwurgzg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uogfpnxv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3adizgkqd.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3zyymnhyg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vlclougx.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3jfnkgnyw.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nhutpwkt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3aeyrjfbp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ztxvwzee.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3qycmpxvo.html


<!-- 参考信息 -->