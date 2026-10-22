代发 wailian999

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2icpuhszn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2xfvywvlq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2urdurbmt.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2mfizcqnk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2sekeflze.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2degiemat.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bnbridxx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mpgsiqwq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ypbjsagb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2jskhvfxd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tzzymbik.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tteaoljf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2srsieztq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2msnrhzsc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xllpkdtg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ahlvvzwz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kcgaoble.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kccboacr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2gdwogmjm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jlydygfx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2evmracoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lskpqqfv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2kofyqlnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ugmxsmlh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wxltbgzf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2wgsaebgy.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gegmhgtr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2okftifci.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rwslsyrc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zheqtqgr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2yceginhc.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2isvqjjjr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hmllpqib.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2vsenotww.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2wrdizhuj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2upxmrbav.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2iederkpf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2diouwasp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zsppcham.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2qpdfotsu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2azpobpgn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2mbnguaop.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2yjekcjmb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2iiezksuk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pfxhgjkb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ebchqawi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rrubqlxf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2wobugmfg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2rueqyati.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2repugllj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ziwmhcfi.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ajpwnaiw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tvhvjnga.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2bsvlvpdm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zzpakvhk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rseazven.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2piiaefjk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lzlsaxtg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2aptjgfuk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vkyehmlm.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2cuvakndw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2kxrcycsg.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yoimrfir.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tbzpakuw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nuqmvtcs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2enuhkoeb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2kqceunnq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hvkpdegi.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zcldrbyb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2eexmdcju.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lsryhmdc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fmxmyidc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lkierzrc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2euzczuer.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mgszsfcg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ztmvjtif.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2doglzxbu.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dihazxbg.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2syevoxjx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mgqesnbr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qobayaue.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2dtavzxzk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2gztdsrqf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2wtqlgaho.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2itrhbblq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ijwwyfcq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2cbmdgfxu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ebwtyidk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2bbmlqxeg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2wvuhblcj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mdslddoc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xjhsaysf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qpbbuxne.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zadqjgdw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wybjmryd.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2fpcfvghc.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2gxwbiugm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nvytrjzn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nyxukgvh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mytypttm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bcwqkefc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fzaprwsj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2zlhhijvu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jalxewhd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2oxdsrgeu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2wnyeaqas.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gdumrxwl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2irrgqzab.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sanmzqvq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fzitmyhi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2jdoblgrk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dokkkjwe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2caunomxj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bvbaubok.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2adxgesbr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dtepeezz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qdfeaisy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tiuvjczf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2oruntdeu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mlsglwrl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2njdnwamj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rjwufycy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2apepuobf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2wxrhfrho.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2mnmnygiu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ijaqzdgp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2xzfulntp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2npscbbiw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2htvpzdpy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2clvppkah.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2tkpramrn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ejyoxykt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xozsjlgk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2mkfursic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jijoccet.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2bntzxazk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2rvrkfmbe.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cucwygfe.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpxoexgc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctghwwhs.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xinvgskt.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2mfrqdtfx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2qkseyfxr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xhprjoof.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kgootaeg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ulbpbggz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2hkhonpie.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kijwcyha.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2pgapqesb.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rtruxsyf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2fxizcqmw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2qiczpuid.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmkoehsn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2tgpfedpr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2moiwpipy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2aeirxswp.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xxnqxgdj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fbbyoplh.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2eyszjuck.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2sznfdihr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wqevplfc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2tgcqpwyk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wpzeinkt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nsceaoem.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkplxlja.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ohthqryb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvceoegz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2woskffkj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cnuykkcq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dimaguxf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2osaifpao.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2rvmjbkpr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ieqopyya.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lnuocnaa.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2soizxgmg.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihtaykdc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2obnrqarb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2zpzfqzxh.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ydylzoph.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2utlwfkex.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2cmrravfh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ibaawqwn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2swbtuena.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2anmlvjlb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzmnlclj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aueutkwt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ridrrhin.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2oxudqtuh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2leingnrm.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2jejphnoh.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2wjlrhivr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2orqdhpnm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tlpzhktm.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fkvadamr.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dvrmfppz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2rahmyydb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2omheensy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2agkemgcn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2inscsued.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ncnsccuw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ksszqaku.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mzqirrud.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2nodrbrqy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2erklkjly.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ohyjlsch.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2lronhncs.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjkkqfdv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2jzixaifa.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2yynxjhjv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhhjewcd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2uwlwoynz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2jsxogrnh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wvdroqwr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2hlpgvdkv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2wdhddyco.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqnseeaw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2zwrisafx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2hjbioajb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2oitqgagm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2saajryjo.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2txuiknfd.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2zhrssvwp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ghvekxjm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fsiorjaf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2vjavexol.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2lbhrvcuv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2oefmmihr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sbygrlbd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2deebavsd.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2quonjrom.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cioqpdjv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wlgasqhm.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2aiqqchbw.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvemszwr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2bwwoxsit.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2djotjext.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwjvzaku.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2iknxfusm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pigmchmr.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2btteahsz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hvybfpmf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dinclzno.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jiqycffq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2qsqswqbn.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2sguwmwdh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gdmczprx.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ewbldfgq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jcjofjdi.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qbwlrmkm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2jcnfghtc.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2nnkyttbt.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2nwsjihaq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2tznpvyek.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2lycghwbc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ofweuifj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2rkqcnfsg.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ipomdzni.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2dqoypaio.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ctmuzjiw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2xhtbpckx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2jatwqhoq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jsjtujsi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2devkbimp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2icjmibgt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2jvalnvwu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ymkvngtl.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2trmgiklf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2dgbfrdyq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2gzooatox.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zyocmmcn.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2npyimazr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2onipwwky.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2sfmmtcor.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uzsyjaub.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2leyakven.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2bikimvhv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2vzmknkwm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2qmihyizi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2hzyhsetu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mhbjnpoy.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vfgvoizi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2weaoysan.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2kvahgdfb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2fndnuokk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2kkhyvfry.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2zcykhyjn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dotzcdcg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vforvnox.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2hcxhsioi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2wewaheqv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ffnbtuyr.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2inrmdidd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2wwcicmhi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xuoefloc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rembfkqc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2djbyfiyo.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xdrcpjbl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2uomtrapf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2yvbxkson.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2biupjzge.html


<!-- 参考信息 -->