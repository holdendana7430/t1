代发 wailian999

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2vxajexwn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2wwreliik.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ymmqrkex.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2gmwxihhc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2aikdovtb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zjvdrlbk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2knsvmyup.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uduhzufd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lbtruqjx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2bsnvpzxx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dpprwgcv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bfciqtns.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2jakswlgn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fazwecvh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2amgffwdw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fiipsbss.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2eqjzrcyh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hbvmehsu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hsgnzsox.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2isiuvvgw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hjspzhmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ynvwxtnd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ecisonpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umdkkasy.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2wjmbpnqs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2kmrmpqvi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mgtplwvm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2cpbwuioh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2uwhqphrv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2oyohcfmc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2rkxsvkek.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rjpzjkwk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2klnxuwpo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2xajjaojk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2gjalzbch.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2dyjquvzs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rjxeyxoh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2nyiqchjn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jguuwcdq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2qzjeeruw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2hsvqljoj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2llejztqs.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2rqdlwzpr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zwrhcsti.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gzgejgdr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ucuhfdgu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hwhsxnpy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2cohhvkjj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2xspoisoa.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ivsheuqu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2xaohtcwr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2wcgirfrg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xnwbspxd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2eysuwuco.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2mvpmhvee.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2uvizjfqg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2mdlmuozc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gtqofqda.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ydtrttfe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2zbtnnqhz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2efyjgtmj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2uhpyztrq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2obytrtru.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zszhecri.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mibghlny.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wujpfyad.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2mhwcwxfp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2shxgznkk.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2muohylkg.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2bytwfenp.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dbvucbqy.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jxmvylnc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2awamqwmh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vqgyltwm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tjgmafdn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2keeorlmd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zpuuvnxp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lzbuxddy.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ryiiouwe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2efmlknbx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2bnuuxmvp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xulptnmq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2nhzbgjnu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ypmwnodd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2iyjibhwz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2rrjeojwg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2zdgpkjhj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2clhopwun.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2wcsifhcn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssnalosm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xvvarpxm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2chfzmyve.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2amoqgkyd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bpwfeagc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ifgdxmyq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sumguqjf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2asvmfegz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ykajewvl.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gxmeaigv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2igbvcwnz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ncebrjig.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cyybbupr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2rfjblnxq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2irnbovsl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2tfxxmftk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2aimqjsrf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xmgsdgei.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ofyztqsz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ivytrblu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cyvqsroz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2klbtmczg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aeewbvot.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gmazsldp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lyqkuclo.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2kerrgzpm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mvjsvmrl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2tulfurej.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uwxvtryd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wiapnumt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2luhwduwo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2igtutyqk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xzssvsxe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2wkedaatc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2sqyngkpw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2edwhgdzo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2jfgnevvk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2jmzdhbbh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2fzebfxbk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ckzkidtb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2qdkxlyhi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2aatkyjje.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2tizytnri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kgjtofgi.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2xolgewbn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tqxfbzxq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2djymgujc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2tqekayis.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuaqbxuc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hpqkqboa.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2aikgoymg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2gujbjxst.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2taeyxinh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ecsaposk.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2sbvhjdmb.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vtsooesi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2bowkfjrz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2cuykzgnv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2agvmagef.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ypodbibw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gydlrykd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2gxytwuao.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bustkchm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yozqtnoa.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2idxmxjfh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2yfqeukwu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2hffkawto.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wsjkibnz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qyrbtisb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2djbyzkip.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ppkcbksb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fqbajfxv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bwbxlulp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2yqoodaid.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2uujuncbm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qtlxxtxe.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eurxnrhk.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrhwiltb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uszmfnmn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2enpzfzgd.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2rsqpwhwk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2mcaprepb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2fbciqaqy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2cmnzteul.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhkdwxah.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2causcigq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2brsbaoll.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbcuficx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ombzihtg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2mvoaiihd.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfvbaqmh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ljfdoygh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2cckxlskq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuxybukz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpqxahxa.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wqvmphjw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fphtqrjw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2esvratrn.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2reardlkd.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2vzzpjpus.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2evzocfnl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2cxyprspm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2bpobbzfq.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mpkynwto.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2muvkvaqa.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vpicapbe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2focehcux.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2asdwsaqv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2qqfbnfug.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2pwipgkle.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2omoswtru.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2tdvegigf.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tivgrtrf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjzfmowa.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2hihputsz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2wvtnpnsn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2jghxmvmw.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2adrghfmu.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ehvqfoqz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2obvfxgek.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2dotbjiea.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2fdwplnbx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsbrhiob.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2owaignva.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2aacwwlft.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2wmwyseqa.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2tjrkwhst.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2nkjirllj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2rzkeosau.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zpvxtegc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2yygjzghl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rrglczsc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2xoolbzfw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2sjxzntod.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2izhfolrd.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2rrgvnjut.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2madpxwny.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2bvvhexpd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rljitjlc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipfbogdz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jpuiddur.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivdhlren.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qqkzitmi.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2efykqdnt.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2typmyqoo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2akblkhjw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wnjcmepv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2irawvpsw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qqnnmjsk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2izyahfvq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tadptvor.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fnjkvlov.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vwploays.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2dtqnievi.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2qzrhwvrp.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ialmnxzm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vepumpxs.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rlcrevtm.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mmmszxwz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ytqvzkmf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2vrjddhmh.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2rgeoetzp.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2zmdkmxqs.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2mmhhmbre.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2jcwklbav.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2txknkopd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2truduppz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2mjobfhfr.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddmncxhf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vdhefpaz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2xqqelmdq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ywwtaxok.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2qfztqjek.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2vdfgvjmk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yacokvdc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2mpsmsxip.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2hdnmffra.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2xcwtxntx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2lgmmwcdg.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2hqphkooy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lbbhafcw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2jnvpvhrz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ixamozaf.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2sxuqzzxx.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zbiyqxxw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kcsurift.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2qvqdwywq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2mshondhz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ufuywneb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2qtfsbssh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aszqrqzq.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2thgrcjgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mfsvqrtm.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2dykifntp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2lpciqdrp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2outkmjnj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2cdzjlnpj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wovygvbp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2hwnovlkf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2uasksoym.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2mnwpviak.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2udpjzewq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2oyldfcjd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2duwgayhv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvvwexjr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dteobeek.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2drnesomz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehzpxizp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2zsmucltt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2bmzlvupe.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rdybgtfa.html


<!-- 参考信息 -->