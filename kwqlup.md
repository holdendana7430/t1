代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lyzwmzgy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2qpjpfmln.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lnduqxbl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lhtigzru.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2sknscadd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2znyidvug.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xsrphxmj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hsbcsbxw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yhxzwsgq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mkjpybtr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2jrvnwhwm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ufcfebiz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2nxdowdrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ouncjzee.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2lfqgrgcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jyjccmhb.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2vnclvyvd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ayeqdpqz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zfvkdqbq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2gyelopvp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yefiliye.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tingbpez.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2zzvqhhoe.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fboazzug.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iudhwktv.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2roagkvoi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2szebkblw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ctucnwqg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2lmtnlxoz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2nxhbhaep.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2cxvttugg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2guxtbpgf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ssnuwfyb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2xodjbfer.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ctwyoxdj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ussxaifi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jazvsdng.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rbntnevk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2azuisklx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2pfomnnmg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2pyznlpll.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2wtrvrhwn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2grfcbntg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2tqorjgiz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jyxldwfs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2aqxwiegx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vtgzlmdn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2itljwzwc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2bffrzfgi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zmbbskat.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2btukygpp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2zvsjkzbi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nkzcyhok.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2yyvcvhyc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lrwyvjld.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cpbfwgzu.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2irnkfvvh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2trsgoyrr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2yjnryfpu.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ccuvzazj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sapkzvoo.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2iysjkqwe.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bjdtltsc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nviualsx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2itafontv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xmuqenwp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jzewcvxa.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sqhseegl.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kqrioaal.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2quntcabz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2zcekfqkr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gseaezzq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kpjzgzbe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jihdicss.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2rnqfpyre.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ddvqbgzk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ysgzwdrx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2adtfpjsd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2wbgcifce.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2tmwmefdy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2iuklpmjz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ubxibdsj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wrzznhtl.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2pqpcxubt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ndkecuky.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2eloqcmit.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2gczchdig.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lslcuwug.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2vzjvezru.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2blmvdngl.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ayrsobob.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2jhixtyqs.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pjlwpywj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xdgstsft.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2uiemoawf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oxtwcicq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ogixqcmu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ooeiwldg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ggsjaasb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cnurzgpx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sjyjujui.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2syshivka.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2wqqlostw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2llyifcxv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dxzuvact.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2utkpkenh.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2zvxmjyvm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vgwskxfd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2umgdguyy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aitwoner.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zzocgmej.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rspgnpgm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2bgmzxydz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2faelqthg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2bvrosnaa.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2vaalnehm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2cspnxuzz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2dhcvfdju.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ybxozhlt.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2cfpepqij.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2yjggecce.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ytirsjcf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2qlwspujv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2cnuhihep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvhxjhqd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ckmgtajl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dhuyvofk.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2xbupkazf.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2bxaeqigr.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2emfgbhku.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hmviwkjq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2udymjkwe.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2swjkcwsh.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2gxzxilsr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2wpcipahc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2amthzpfo.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2qhkfgxwe.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2euamwivc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2betnjgox.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2llnyorws.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2knbybcnz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ruqwhsmh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ufeqquca.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ewlwllxh.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzwuhaov.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2anccmrxe.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ozmbnriy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bdkremlg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mkoyoxhj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2iahnchzy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2mzohythr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2lnljwlzb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vryieioh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2cojkeloe.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2gatljyhp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wlrbrdjq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ahnzcsfa.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxgmvfqj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zjpmrovk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gevfpnty.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nbohygil.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2pgxctbcc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lyaqcjzf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2zagddrwj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2aqcpxtjv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydrjvfce.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cxswgbfi.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypjwllhi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dnnyqfgc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2sityrjdp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jxzldlap.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2wbaqtwty.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2andhpaaz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2xoywokwa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vwygfsla.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpxcyphz.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwlqmabo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tidgpjnr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2uhsyvzvm.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dhalwjls.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2lznbqhcq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ukiahtxz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2rcqnhvpf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hkxncice.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2commpcgg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gtgtlqop.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jpvcmcar.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2dhiyxypz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2qspbshcy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2vdibgxyg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ysjdogtf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2zosspwth.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhamfkii.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzfsmbfe.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2tmkbwcdh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ladlgrlb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2fjgreduf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2nkrnlmcr.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2fcivxfea.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ktjrwyhy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ucalixkl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2brxaemrj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2adchonxq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypanvssf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2mcvmrptj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2hseeuwrn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2czbahzpi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2evhtpiwg.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2tgxopxsi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2zcbpsxlw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pkwcymhn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2iqniblse.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dgzccyhc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2hsghivlp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2cwpafdaz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ucskwada.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2nolnrslu.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2qwgfmgcf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2plevuggm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cekyiblg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixrsvypx.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zttzwnhd.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yrliuryf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gaeiahww.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2kvzuyhzl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2pvzkhesp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2uctsrviy.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lxidwyjf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nozzntwt.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2otkhzrym.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qfnztggc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yilpytnl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lzribgix.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vdklnmsu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lalznmmg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2dmcbqegk.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2hivsqmpe.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uwmqwbyz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2paisqtuc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vkkdnjwm.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ljlrbner.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2sdntrpel.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2kxqneaai.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2tifflqzx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2gaabealw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ktedeleq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ccqzrexv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2pwijgsdj.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2bntyidqb.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wpsqchmh.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2hziavfhc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2fcajbtsf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2qnsjvihv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2gnlqjieg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2wydolhgr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2kqwncgfb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2fmzczrdb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2uoyxcizd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2nfaixoco.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2tjpwoxwm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ltfsznvm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ejohskcs.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2dxjuneyk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2urdvmqwi.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2dexapkyt.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pjdibald.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2uuuthuvc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ymuyjrtb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2slhkxnzw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2dkotvmoy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gpjjfzzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2krjurair.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2skluddzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jknqtlst.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2mpwlbnet.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2uwecusxz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wwaryzmy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ayhpuoin.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2yqgfogih.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2omeceiae.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2zrfsjfsi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2hsvozwhh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2iyqlsish.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2grolulue.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2bqmnhiyb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gcxkigyh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzqjttdp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2npivvrgn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2roubvknw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ixfmyzur.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2zkqysrtr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zyrrsftp.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ayignbso.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2cyypvaar.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2feorbsob.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gsialqsx.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cgriexco.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vhzgxasm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2czjhbthe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2essgtaes.html


<!-- 参考信息 -->