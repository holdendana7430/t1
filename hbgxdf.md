代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nkslrslm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3qallrldf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3aozcdhel.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3udtnlhqg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3nztqyrxh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3riqgtfrm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xqbqsgcu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kqwfdcuq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3uyhjgewx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hlzadvhv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3atdfbmha.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vxhcgfpy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dcwuuhrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3npuclfhe.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3wsxuncln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nscjsmlh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3lpeopgji.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ipumejba.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rdzditsv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3bcggvwrl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rzdlmcar.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fevrzjbo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3glfitbjz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zkvljizm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fjutugds.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3pfybunef.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3gbazowwz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3jobbmvak.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3masghrpm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3udhapeqx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3htywbgon.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ylbzhmzc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3lsnfzvjp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3felejtro.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3kmnctqpi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3iyfqkeib.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bgtfyzbg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pfgpqutt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uwuzylkx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3dpyuushm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3mvbuyjea.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ypssqqef.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vgblgqkj.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3qbedavdn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bhlqpqcf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3sihztuzc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hcihiirr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gmvggmgy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3hucsfckm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mzmtcgey.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3hxhmdshh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zlcpqica.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rwpolqmo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ksvheygy.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dzysxziu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fkpzpqwh.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yeabthzd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bnskchjd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3jitnacgf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3opjpxcmu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nhkqptex.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3pztccepa.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bkgycguy.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xhbdlish.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nwaivupn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ajbnhcow.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xaxsfwec.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jssusszo.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dgfjwhnq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3huxhgmih.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3qaoajijl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zwfzgluu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ltctascr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3nmtjitos.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3lrpacibv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ytgugbtu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3olatccjb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3htrlzwcu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3zubfpyff.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3rkhneccs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3wbpysymi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3dhurfyft.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wgmvkxay.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ihrdytdg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fcwxchfk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gqkjptfq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3vqvpwjta.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ycbfrhvx.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3qypeyosy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3satflaay.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nhkhaoqp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3uljfgdvy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zujcbsmx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xobqmyfa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3cfliskie.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bttcgdts.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3apouhnih.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3iyhwtfbm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tiljftlk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3phqfjipu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qzewsqcn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qwjofere.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3mhilmhpr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gsxjilxi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gygzivsr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mewwcbhn.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3gyjhpkio.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3leyknlao.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3cnhpgxdk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cwueuouc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zoaklmve.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kesgrvdb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3bubhyzjx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rnmfuywz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3nbjctijq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3hfnsxkjy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3mkdvvudc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qvuemakw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ybzivsmo.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3wawkakjy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3dmjewgki.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3wmsbhqoq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3qittfgcs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3mqrzqocz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zloetrhp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3gkndcvax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qxlvdwbi.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3fkssucnk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3chcrtpuv.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3onxhizfd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oblxfbmv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3geecvtmh.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3leayjzsy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3koemklye.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3sxcdvuiu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3udgnsxws.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3mvnrupvj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3twzykmbn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdxpogzp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vmjymeyn.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xcbrugmz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3csaewybn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3yqrkeoje.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3irlaoggd.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mzilqyak.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ilobyjlh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3pwtihkdb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hvjqzesw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zlgyfnvi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3azlcsjth.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3cscqjmte.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3xjqmhkpx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gloifjmw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3olkkkxpj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3stzbnoxm.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3sswhtypv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iywdwory.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmpytowq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ejzwsdbj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihouqryp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jghatsgi.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ntnqwszp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zfjptntr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ifkqmjfz.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3siddilcr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qeudovlj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lnbanqfw.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3igydbrlz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mpnnipci.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3yrjmlbdl.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vrqvhdpd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3uihatino.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3iugkalsh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3wcdiipkv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pjuuasoy.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgmrbbrs.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jssgttbu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjjolzfo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3vgtzwumo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ikumdjab.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3mhmmlfog.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3njxlcwlm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3sftmwbah.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3qiiamqbi.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pkmolzir.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ljczxtlf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3diyhvlxv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3rpikohke.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3jvfqtert.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3abqqnccq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3zipsjvru.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3xvaeztkz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3equfyemr.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3owswqdhi.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3pnwwigax.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3asgrxwoc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3bugepcrh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3xprccpay.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3njwpknag.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3dxikxvaj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3qbeppjku.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3yshzurlk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3vtfkvgop.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3uebffyhz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3awgpgkte.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3hiugimga.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3annbbfbg.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3uewwhjzo.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3onysqanl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3elsjgwug.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3iugzwjuo.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3mgdqvjww.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rrsnfyil.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3mrccaclb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3unqqpmql.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bxsremcp.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3axercaqf.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3yjcsshpr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3khbqvayz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bueotrug.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fjyqtcou.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eaumryzk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vrrqqybu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ujtuqbcf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3dohlmmvz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3modldypi.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3tmrwpopw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3roabjjdw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgymtbjj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehxdnjgc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3byuqfxls.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3txobjdxa.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ftkzgnzh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3oighvaum.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dbyyblpw.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3kiqblqdi.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3msokwjxv.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zhixofjm.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zuooojtk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3urhffsbq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kdiwvhjm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3amvyyhml.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3aegedgrm.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3syrdavyb.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3veqlylld.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3zurbzbjf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3hmgcgiph.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3wurcgvln.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3pcpadvfp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3acsfsgym.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3frdorjnl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3nuvxxrej.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3endxhzct.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3djlrxinj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3lomzmsmo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3sgojlhgf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3cgskgqrr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3yocbpzvx.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3kjwgajcu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3vmnjvpkv.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3qraoykkp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bxusmtnd.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3tantokol.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3mdptfxuf.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3nwtkrnof.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3tebguzdj.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vctuxxna.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3kkbmsloj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3fhczelik.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3axyoxfpr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3owzlvvtx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zzpgcwdm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3dximyumo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3agphxwjr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3rtakkjhs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3qpejlmkk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yttlmmdb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zhcihoyo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xylnxqhy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgtvpwoy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3mnoadprh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3euuhphpe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfjhnzjt.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ductsjfq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3rqkmcjld.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qujodzgt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fcsqdyfd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3iwqcxzqd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hbderecj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ljsmjomn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3opjvlytv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yiwkcble.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3faeehylc.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ywucjlau.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xfevdtic.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rifhhftt.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vwjudxik.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sicxffdf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3mxvippic.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3coasuozu.html


<!-- 参考信息 -->