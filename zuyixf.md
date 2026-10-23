代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mvwuumox.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3dgbvxjid.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ezaosmyq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kiipyulx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3bwcbfbmm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ymscidcz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ezfnoncz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3uiqnqzxn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fbduurqr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pxerghpx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3sdfbaqsw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bcoxttdb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3oohnwezo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gbzxhqiy.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3cwsekfzg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pooclyhg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3hgcubvgu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3vjwierlw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jmukwpnb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ffkfhdwt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3clplfbew.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tdnhsksj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ptmxllzl.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xlwiojaf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rwubadcn.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3iknxswxx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3lccuvahi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3fldmasfg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3bfhcnmqr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bxzkroxt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3txdamfmx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3nfzfyhhh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3cbmrognf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3zrkhpidt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3jxglpnjx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ctkoltic.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hnyoamos.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yevsxcud.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nsbwzdhw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ukxoebpq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3nghlyoan.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cxaozsrn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bfymhbad.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3nahxtyng.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jyqzqolj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3uiwlsjbn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3fdgakvje.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sclexxkc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3linmoeyw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fvqkenzy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ybuwjlau.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ruwljgsi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3eyoxodom.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3wokcynqu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yxmssnzk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lfficzqm.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oqpfkzhg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cflpjlvs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3sdswkldd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yskweiai.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zfqzojii.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3unlkpamd.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mzqrjpcj.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wfhcbmew.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jspeodcp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3irrihagv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qszxbmib.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xursraox.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xxelekpp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lkpnssam.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3nxryzstu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3rjksgxrz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3pbcrrwnb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mnznzpgi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qhlydimp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3vdbqzdac.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3sxmtdvxh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3bawyxzgg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3wxmipetj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3yncfqqxc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3yheuqnyc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3othsyufb.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3egfyalhx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ikzwlskw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bayrjyaj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yudldfgj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3awqzovnh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3llwysgtc.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3dyplhtea.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lbtfmxlh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tfapwlww.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3egusvdxq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qhrnzgjw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dqmxvchx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zribtjib.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqaczlja.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3qlkmjhyz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3crrotmzj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oyyuklkz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zaszhtgz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dbwehffb.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lmbzmpwl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3yymfwtvs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bgtxopan.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aljnliul.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hrkhfllc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3lyyfpgzm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tliddtqm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dwilteen.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3elcdzdkx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wbfimzyi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zaevdgkh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3muzgdopd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kkiyuehs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3npjmbsbg.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3qwuijhfq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3uciqhwev.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3erwxstpp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3vkgpdxmh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3kmdwtidp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3yhrcdolj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3mzhcjoda.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3aeidvcmk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3gulairas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqqqwtnz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3djjeyees.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ohtruzau.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3wbtjqrlr.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3mckegyya.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3fihkicfh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zmkhymjy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffjdixoi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofnjcegv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ftvyknbu.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3mkdpkcxf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wutyaazb.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ymebdyrl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3pskkzbbo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3gdtzwofx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hsxqxtzq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3zxoujwla.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jfakfoqu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3cluhsrub.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3iwwctxax.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qgxlnody.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3gmvzwrsx.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3fhegwfhc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3krbpgdca.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cctbvfeh.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3lwzprjgd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3qaaaubut.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3yyuhdbso.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ilsluguc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3wappqewc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3oreosrer.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jbfvsfpo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyqowktq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylkdavbu.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3chxnzayb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hulbvlez.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xbuwwale.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hgqminjq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3svciidza.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3aykxbjgt.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3iesrwebn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tsfpajum.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgayqiuz.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zbyhzrlp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cnvemzsi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3mnvwpqpw.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3xcqbbyru.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lzzdtvdm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3kxanbqok.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3pnxrench.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtctqysm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwtvfyll.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgsxeoar.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wfcmoxbc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3blocggnr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3axzmwkqv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3oxtqaquf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3zhjkoydt.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3tzqalgos.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bxtlekjn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yngrzufj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zgsfzona.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uuvqrjvf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ebhdwhrw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ajcpzhte.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3gkgumwsl.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3oiswfjks.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3rmzxlcnm.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fkpvkejr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3oirctexi.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3tnerljik.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nyskxjlz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3kbhdykpx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3xdfeinyo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3vcpeykrn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3gedoiaou.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3bfqdkafk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3uuenjvrf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3istemqdp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3eiwzvrca.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3udocyrpv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3wmynpzyj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3psapyhzy.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ysxdvgtp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3dyzfmcgz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3xoclcpdi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uzeasqml.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3llqqwtgm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3psqjepuz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3qxnsxpva.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3vpovpbua.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lvmcgcus.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3hfpdkobv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3vnciuzgf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3pahyoyfp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lojvwffk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yqjhxtgz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3zguzrzyo.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rmfnunvw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ylwirngb.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3vsuglbrt.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ttbtgcng.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dcnqibmo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qqeufoxi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3chtfjnme.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fvmuewno.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gjyepaly.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cixytjwx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3eimardxw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fnfugwrr.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gcttrdxq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3glbraqhs.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3elilntsn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pfyvpojd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3igraguod.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dqupapsh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sagnyxfc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3gwcahibn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3knzodzds.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3suyvwwun.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3gojlihzp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3dwqvmprw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3fywvejqq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3syalxuss.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ilmqqikf.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3xwnojpii.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3omqlegsn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3ojwnjkfo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3anhvpqiz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3yqntsprh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3nfglhybl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xacazgwl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ubfnyipi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3hetpdifq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3gcnkszzw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3cjkfbyrc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ptwsbahj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fnfwmrem.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ghuipfib.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3susopxcd.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ykvqrssg.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hnoevkqa.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qrjkhdry.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3spihwezm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3bsmexjbk.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3unavzfbh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3yyjawtsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3euzbbrzx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jygjagrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mwjydsdw.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3dkxbsstd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3pzremksg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ygynztxd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zmqxpczd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tvanjtyo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3xrzluvhk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3dhfkxpjs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3pfrrzngq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3byjnicyx.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ztubnbuj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ersddmks.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gzcafiuh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fbkmtlsh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lpoyhcif.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ausopaus.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3nadmqljd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3rmeiftif.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bqrgyegt.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3fraltegt.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3lopiodik.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ewysinlj.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ertikrbi.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rmipydeo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tgpkoskh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3kutxbmuc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ogzgfbhb.html


<!-- 参考信息 -->