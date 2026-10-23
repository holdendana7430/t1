代发 wailian999

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3jcdrevdx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3cvolccyj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3mlpvnbbt.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3lmimvqvu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3bqeczoik.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymoujivj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3qhlfblhn.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3chdxyilg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3prvazhja.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zlnsphum.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3tghmhond.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3orqzbrjy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ttvenygx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lnaposii.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zbimdtug.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mzpvfwid.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ofypojee.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3yrpkkeov.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wntctqqb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tyktfmnx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3yxgkgqkl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ofxwqvox.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ryxitnox.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wlrnwzpg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jotxlebu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zuspkoaz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3usaobbon.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3keacqhya.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3eajymoqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hbdymtyi.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3rfvxdnbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lbfrpprg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3xhmoehpf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3pvmbpidz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oespkgbr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3petrruqp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qhbyvxcz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3koxxzlkb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3vskzarxx.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oyebstks.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3edrfrdiq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ewbtfeoi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3untsiqyp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfkpzzqg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jbmhwuhd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3afxpdukj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lrqxuxxk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3oqqycwzf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3dbimicua.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3xpmlkcpc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3kzilvamf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cktmyiyv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fpgdvypo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hbgctgwa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zjwhhfkg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3iscrrwis.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3znckjuzs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3cckefaxb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xkbiqwfz.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3euymxovj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kpetmazu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3wsaatfcf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mkrazeav.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3behufpmr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3xsexpmep.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3kmzvbqfz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3jbkfuzwp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qinvczlb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ijbfyinp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3wjsukdce.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rmqmkxyn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kbkjqdit.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fswvqpty.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ywjhqfdl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ocwtvntn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3axvjyovz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xjqjthle.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ndmpzbxd.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aqrarosl.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xuohhewa.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rlqkfnet.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3azjplkkg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xvantmcj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bolyvbng.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mlkgoift.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vsobnowz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3jyoodkht.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qtyrktuh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zggsnifn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ecvgijoz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wsdvlezp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3wocpitxs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3sqwfjyjm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3cexznize.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3jnxovbuk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3aufjurqv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ccwmlicy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3mufvfvwz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ygnqbjit.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cbzjssjx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xhgwbndv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3udeeteva.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3nzgxmccq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3peczgvhy.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3qwjbubbc.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qazrkwqp.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uhicoabl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3effygaxr.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3mzszciib.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gakvynwc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3fjhujxyc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kinjivho.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3lntlvwic.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3nsgvoeah.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xhqboyqk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gticbsar.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iivizsaw.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vhfwfpnr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ujuynrqk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ythmgvut.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uwjzjrhj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xnlvbfky.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3qwvltwph.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3eguhclmt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3orsfvsah.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pcmwqbby.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hlvrgnfa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dsvhpglg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ksiqyxjl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pjqwjrja.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ajfzjezh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3fhupwmnd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3snnnepxv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3zzergyrt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3zygmalfw.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3tmvkfsvz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3zeobcydw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3flqqfwka.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3gbsipujb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3liilumtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oqjizngg.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3qnxbsxsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xykfsicl.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3lbwgdvxc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ourjugan.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3feucjfwy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wngfhopv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3isuruiyb.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xivbdnwv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3apexziel.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3wrfisozb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xbzfmqnv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wpijwgfq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3cvwggazc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eyvtwxvm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uztzbhvl.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ldvdymrc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjjdlilg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3jnphcxzp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3fmdnqagb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmpjtyeg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3kdqrtsky.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ktkfmkfl.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qpqcxhds.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3armhdkan.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3oyjglppx.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3yarjpxdx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3mlhvymmm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gttnkghl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3sibyqbol.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3nbcicftr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3egkyayrq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tbqdrgza.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lheqxqzp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ifzktljp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfragbcd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qtwxngeh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ygnaamtv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vtbkhpis.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3upfnniaw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wmconhkt.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dnstqpop.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmigqdzl.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3atfgykxv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpqcgrlf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3rpxezldf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hhkbkldc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhdjesgj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3prgwqbfp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3pndvzxqy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tjubjfbp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqqfeglt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjbxvhzz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrocoaeb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3asmgexjm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3aluwnlar.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3piwuokjy.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ssgjjmcl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3nerfzohb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3nzhfjktd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fwekexrl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vrkddnhf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pranycwg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3trmfduod.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3zsuwhnzz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xijfsrzo.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3wlmzkgdw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3qbtjllbm.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkcnbvei.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tnhkxyjv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3unutcsvj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yyqcffrs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3lkdworns.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3iuctddyq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogfehjtv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3uqnptphe.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ikjpsckw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3dabwgtpg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3eerhiamv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzmdrptz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3itzxxkys.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3xaqmaklv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3iwwisupl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3zjireyhe.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3inlsjpst.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3qrhtfzzi.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mswebzhi.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ifwwrill.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3chhucxqq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3fgxnoyqs.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3muevlxsc.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wxxvfgnm.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3lmummgpz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3yahuidbu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3dyqcadoo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkmtpxmq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3olwydgyz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3nvepdnxj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ytzqrnys.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zanrauvj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3gpahsppo.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3xwzukotn.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3jfqvagle.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3cxvodtuj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xhiwiqvd.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhvklyiw.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3orjlugob.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xiwwzfil.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wzbuzssa.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3yupumeke.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zgbkupjq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3zhcvgmln.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3hndtymug.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dgwqadnk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vcnpxlol.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nkrwqpvt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lahkdvpw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3morlykcl.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3lwgvrdfi.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3syxouxsp.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3hwhbnnym.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3qfffiift.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3sihhdceu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3qinsalzn.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3pznzmcdh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3etssenrt.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3hdszinam.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3lgmttxlg.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3uzdpfqqt.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3kydjfhwf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3cpoqmvtu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3osxivkzx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3qbfzrukm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3swryftmj.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3euekbbxd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3tukzhriu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3shwnldel.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3poomfntl.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3vjpuokxq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3irfsggtn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ghqnyllw.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zzpgcmsg.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ogxmniya.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3maxzeyky.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3mpfsdhho.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3djusjmjr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3txkufrve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3otahniri.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3wtqavbfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cutsvher.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3cinzzixj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3woksqtru.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cexwsqda.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xwtjpzez.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3wlgqkdnn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3oxxnyndh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ayhwsmpy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3xqhwpjfg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3fvhbofrp.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3gwkpbkap.html


<!-- 参考信息 -->