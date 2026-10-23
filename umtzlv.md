代发 wailian999

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ttkpyifg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3efvukjnf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdiatliy.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ndwbuobz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3spdzvvup.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gfipfjih.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bsclxqhw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3istrrbmh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rldjjuby.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3gxxxlhea.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jbdkamwf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qiuaeepf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3srkqfsoq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3bndwflol.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lbcefcgh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hiolrasu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3aqkxgnxg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3uavjpbfy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3vrruujzr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zmyyuxrk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fqomnxfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rdofjbex.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3wnrfbjfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wkrtmzqd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3gyaraiwh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3nqzqxquq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qclxiwjc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3vmymwchi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nnjstqrt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3amgniybe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ubslhaty.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3stowtdna.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3scuqxqvk.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3bvzeahjd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3pafgakba.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3shwcatza.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rpppilva.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3horelnxn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cdindejb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3jzlrbxqw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3crlajzhu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ykumyqjo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3mnzqwzxy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hnwlxzin.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3odnwfgfc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jvxqztvu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3psvedtet.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3cdquejep.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3wlftyxqj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pxnujzel.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3todiotla.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3uwhgriuf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3eqylkprh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3usxhzfnb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rzynoqgk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3myzvqaqw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3jaoztonr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xphembtc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3wqkfpnhw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zhqylqeq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ruddltnb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ibicpklp.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3graqbxsw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dzlvxepg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oomobngk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gwduvxmz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3mnyqcchy.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ussfnzqw.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3axchksnw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3jwzxudeg.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3panhlyru.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nabwiooo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mijnjjrz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vhdhimco.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zrjvssdu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dhxslotg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pyenwaha.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3udwyjeod.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3jnlwkohe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jcbhewrt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3tsmrownw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vuhidrvk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dvxozrao.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3xgpqfbah.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3kdhdkhmd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3nxsljtvc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3zsijoicv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3tfsjctbj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3mnoayssn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3fyvgifoh.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uhazbfit.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zdrwzxvs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3zvjdbyuo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vtyvnbrw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3xkbcobir.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3gzfyoqbf.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3giosihhd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jvfjefbt.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rmkppejg.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3sixkbhms.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3yyfzpuot.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dofqvzgq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zfysjopb.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jmapopaa.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3pzozjdsw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3rhohdrgk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ousypwvs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ysxkjnqe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mwdemflz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3grywnrga.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3qlicbqtf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mxjnxuzv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sazsxmws.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3onhrsuax.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3fapvizuu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3epgkdicd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3thrwehnq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rmrcmffa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kfsqhkpy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rxlpuvvs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3aidwemjl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qupmxkbu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3rcxrccxm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3bkqspmzb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3wcdgnucu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3pkejwiun.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3adkkpbco.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3jqimloes.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3rjcxnecz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3dwqgwlfl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3htszbusi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3tkmghvpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hvswiium.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3zzyisrbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3botozuwr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3divhsmzj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3atogtquk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3degtzjsq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3brqpzpsi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3blyzvotf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hijzizbh.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3emcucnzo.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3cbuwkebs.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjgtnfip.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3xwmwzysu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3vokmcjnx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hiypdxdb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fffrjqpk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3skivekbf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3oczrokgg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3kqsszswu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tkjnlblo.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ltpbjiag.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3qhpbxniy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gxpllpyf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3roxlrlma.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3whkrwxmj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3gvbjsoyz.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3bxtjxzca.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3aebwyrmw.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lgpnmhrj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3txllxnzw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vdhhkmvm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cdfvhrxp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvujeacp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3grgczviu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xnghcgrj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ucqcmdex.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xfgpieah.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3utibdtsc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3upfhvmqc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3rqswrtlu.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3qumuohaw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzrnferb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kadgmqbb.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3axeejaug.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmsqlizn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3kbyzcyqb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3bspodron.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gnimyvng.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3rsigvfoi.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3pdwvejwg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3riukaqzg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjbtzztd.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpycmftk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukclvmrf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3knrsjeuw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3wswkqrjq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3xrwzvkch.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3jpeydady.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3scuseqwn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3jzjdwlwl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ygsfjuam.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ytkxhglx.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3irchtowm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3uworelfe.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ntsmjkov.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3aymcolbo.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3iqruutzo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3rsnqlpvh.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uoacmlcl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ldniuamk.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3mnmcxtfp.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ybmgjeve.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3wkfkisbf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3flvfduzj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3lutziint.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3telfkonf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3auochbdy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3vdqbqtxk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3xsgqhpbh.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ymekdxbx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3gadawbpb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3xzvnfcci.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3hzyrqvsa.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3lscwnild.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3wribxwpi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3sdlwzzfk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3awkjxgnr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ihtcxyjb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mgjcpcve.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3kzbawlzd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3qatvvivz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3uwlyimhn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ywzrfffq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3dkwrxhhn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3apsagaif.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sngngbdr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxlqeyrv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3atafkrjt.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3omxucrfc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zatoszif.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3tiommemo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcffnety.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ftbvdiak.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xrpmpkfb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzuipgkm.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wzsviycs.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3krcomcfe.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztvenfyc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3shmqpvlc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jtobvhqm.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jdihtuwh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ggscbnhz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3mvwbldqy.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ggzpboin.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vyfeuwgg.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qgygftwu.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xkeusilx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3sqnftwft.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3pffhwzrd.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ltoqlakr.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3sepdhxdu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3gdjahrwy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3daeakpkz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3lvblisip.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3qpbetnet.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kustehxy.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ewryvisa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3qozbtypg.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ptbtoqki.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3bywbrjqn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3bsmckvtz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbcbnoqa.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3zmamalgw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rfyqlwad.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3crcdmkji.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3yqpbftzo.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3xfdtjhpw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ckbracod.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3oinsdrqc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3thpwqfus.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3jdqabfna.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nhtlhhsq.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3feiscumo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ootutdfw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3fsjccwuu.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3upmaudsg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3loydbzuk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uhasktuk.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3tonvpzfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ksqqfvxb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3tvhuevno.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3xfcxwrcz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3sscreaeg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3lzlwzlmb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ouzrvntv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3tziykzrw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3fjujarie.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3uichyhwj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3brohyzan.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3uwmbujqv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3dsdajxws.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3drwnsuwp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ojwehwrm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lazmbcmi.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zngfkviy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3jipgxemw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3jmqxfzln.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rjtywrmx.html


<!-- 参考信息 -->