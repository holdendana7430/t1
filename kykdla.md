代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2dsgnveud.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bjqwhnht.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xyxlpdwd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fadlwyvh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2roqpaftk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2wglndzst.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ynxwgkfs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oqxvhbds.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2dgpsgkyq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2dkderrgw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qlkqwnyw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ejcnwjzq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cvmuzsfh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2uvklrvyu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2sxxdcwvv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gydkizvw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2szfoddvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mfnvfxkn.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ujghkpab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vzkcxitj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2vvisdtrw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2kftwmkxg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kbteagzc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2fhjncvpv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mradouqi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wetvcymw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2omenltfm.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ebahyffn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2obgjwnde.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2bhxxtnvp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ocmemdwx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2nzmpeuqq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wqqagtmq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xqglbzpa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2adtnaabv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2lysjbjpw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2kqtktutx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2vzpbgwam.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ycnqpjzi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2rlimrpdw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mmtpdaft.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2edlaayvs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wlilssko.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2nrmxydvz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2hzotlzbp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zqvttnyd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fiehwfug.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2fwsfzhwu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ptsomqwv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2iizzkndf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uhqrsjfq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vrvvxcpb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2jslsturl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wdpxzrrc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2inxiwimd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2kstijseh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2dquegnuk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2byewhcjl.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qdevqtvr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hdlkappr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oxcueqaj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jcvofzam.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2uiqnzpvw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tflaionm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rzwryufm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2dztoerzg.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dpmdehqj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mektrxyz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wdnjranw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ixxbmmqx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ifxviurt.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bojgewdy.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ajtelhim.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nfhdwsdi.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2olmmryhf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2vprbkicj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2pnkroubq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2hwfwziiy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2cjfvwpml.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2phnwpyxo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2srqurlmy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2jrhhejpn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ygqbxnik.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2dilzprsu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2snkhuboo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2laufhynq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xztetwby.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2eiavnebx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2uotujyzn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2abzlpgdt.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jdjbpblg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2lxvcspyw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2eytvxmor.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dbijsmzg.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yogiedav.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2odufosga.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2igjkieph.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pvnhmtki.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2hgsfoirc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wdpoeepa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2rfoldwiq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2borhhvrz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ctllylbl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2peteeiic.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tieogmdt.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nmqgjrgm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2mvetywyx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2phwbdfpc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lynapgwv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2opdhiliw.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ueqrcuaw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2clhzyqfa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qtftcnoq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2csnlyqjk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hfwjujnv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bxtngnus.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2kvgsyagt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mawwtrqd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2fxjsasrk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2kkrtlvka.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2isdovfwt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2juvqjatx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2gedkqtgw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2kvpvkrmv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2phdvcqin.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2dkydtiii.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2fwjevrzb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2fsfsnkku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hzvfedcz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2aaigfufj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vawijzys.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2mahigjbb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ciyykxtp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2eeycqjbv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2kqyovkjn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2uplccrxu.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2adcftbzd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2olgdcgic.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2xtqsfrry.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmtkuvob.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2shisenqh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2txzdszbm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2xtqvcogn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mmglsmyv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ftiqphrz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2chodzyjp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2suzjdtse.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2yqkgxvwu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2knjsrwlq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ybrubofg.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fqxvsopv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ifypdugt.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nctzxhrm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2zsezadct.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ipzjlxqs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2adfacvca.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xgdmhern.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2feclrkpf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ibrsydiy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rtatvmqx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rrtjrmvx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2csmrghuk.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqagaxmn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kjpomjce.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2idiycgqj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ibataosv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lipaywud.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2uysvqhir.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2jhraphvt.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2leiizfhf.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2adimcdsy.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2oumxbbjh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tclfhara.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2fdfvkunu.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2neayszfj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdvybcjl.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2xrrrniav.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2kxlavrln.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lzxwpblq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcrldoxb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbgttbki.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zhflwqqe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2rgygreum.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ycuthjkp.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ozkxyuuk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2nhcvdnpz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2nyyzunzd.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2suopbzzu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ionauohx.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rfpgzqdf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xxlvnyzk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2wipgxjhp.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2jwcvzaru.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ddjgbaxf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2snsldwju.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2alcjsfse.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kjjgmquu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rlbwbjur.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hipxwfrp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2mxwjlanj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2aklzcvbj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2urrwpmcr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rhutiasx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2fbmpyauh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2btstciyy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxoqnngt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2utkgahcx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2mrthhlzm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvmjjygi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2hdkbgthh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2irxiwegk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2powyikyf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2cklnnuha.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2mgpacamx.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xggmtuxo.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2xmztlhbb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2teksmref.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2creqaptz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2hymsizat.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rpehdwyf.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2akxbcchz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2lkjbjkny.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2rwnvdcao.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kylctxnr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ahmwgctz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kekybhdd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfkrexlc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xrhaaosk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2npphznkk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ngciqopa.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ngcqimlb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2twicwrwb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkycuybc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ninfpilc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfytifts.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ckfiibnq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hsnaeynd.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2octjbxzb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2irjeazwv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2jxskcmje.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2hifanavh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2doyzogia.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dczxhzzj.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2savfkfbc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mopgsdrz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2sgculitu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2zqkropia.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2kyfyfjzx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2prdtftln.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2frzhkbre.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2nadminmh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ggyfarth.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2drkknraq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnidwidm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2edjdsiyn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ctnyxzgx.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2qjuxcgay.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2cvzigomr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2kewzxash.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpqzidjt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2dbikoytz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ffkluamu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2fkfquguk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2awiiffgo.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2xflpqssm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2eisceycm.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ivsgsdwv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2nhozwdzl.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2rllqlbec.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mijlaxrk.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2yjrvwhhc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2vaxsnpjm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2qajzcshv.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2bezcvmvw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2hivgzfdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cgmbjwtp.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2qaxqnosy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vsnbrlkj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2lstokmwu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2njatodig.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vcfmscqc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kvwdhian.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2egtsrexf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2rdgulrhe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2dosgckeu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2bzxbmrkj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2xzrcupmm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ewxjivtk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2xvcztidp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptaapvbv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxhljrcs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nsyeacng.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivvlmlaa.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2zzuifwbq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2oifluadx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iarwhxmk.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2arefpoel.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2cgkghzcw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cyjgwrza.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mxwfbjrf.html


<!-- 参考信息 -->