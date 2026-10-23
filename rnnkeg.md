代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3sfgbzswx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nvkpffnn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3xxtkgmnz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ozfzetvg.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qhbvvqwt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3gvnqvicj.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hydxehej.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3lklonrho.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3dktroaxg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3dmbwpzxh.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3yosdwbql.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3dnwmcalp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3kxlyszrx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3txqlxspb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3jtwaxkdb.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pgbwiicr.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3tnuhbxqz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3nobiergr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rdqogfct.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3vzfdmrej.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3xkuumpox.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gnygrzia.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fynfgyso.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jlqtnhov.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qywbtlha.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ukbbqtbn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tfmdvbid.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qveqycfk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3mrunjszn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ukibqrzm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3namcovfe.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qfbhjjju.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3uoaymnqc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dceltgqy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3yrcmwcdm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vhmlrrqb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rlriahjq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzjeftne.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3imiiuiao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gdukqrnk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3aucsusmd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3wmlqsjka.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3brgfthrx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3yygrqusy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bprmhbjp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iyixhpdy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ffczcgli.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3swulgvch.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kcrtgjyl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3miyqawlb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ndoeahuq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzwoqvol.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zidoahhf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhtztswi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3telnfdpw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3toiexemu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3nmcffrxv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3prdhamvl.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3jengzqbg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3fvdcbmzv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dghavvbp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qekhzbmx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ohhaqgkg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3euuwzjwh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3uhojorfm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3wkenbzgr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3cpzzwhfl.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3brzijlds.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ptlduzfo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3bsfranak.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zunkjgbj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cxapgbwo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3oawqkamx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ctlnlinc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3djxonrxb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ysuvqkjb.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3qtalwgod.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3uvsnndft.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3goelpbrt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ohbaugre.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xojherxp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mrtyvxdr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3xcosybzk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zedgetvy.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ebztmtop.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3jhwmewcv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ggyrxbij.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uakswugh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lpxtvyvu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hecjzsae.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3meejryvc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bjdmjgii.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ayalghay.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mxsdnono.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3cqjhsblr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3uplezaru.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kaiefdrg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lppgivnt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3pgvmissy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3zuruvhia.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3izcotere.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3oaokvezv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3zlzryqwn.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3eksgpasl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3qtixfcya.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3xohzabfc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3dyhlzbga.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3dkexctqh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xxjinxdi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rsxxupft.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3brtaltat.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3qkkqyjsq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3bpyhkcls.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3boboxzhh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uknlzeuf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3pefiidfp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3obyzdcxz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3aowdbmau.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3rhstiove.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tqbwjezq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3yjnqplyh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3tyadpnkg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sbtmvtrn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ghnbslxh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xajmsplx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3irjonfgv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3xfbqslnh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mjsdukwk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3txfgbojv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hbyiorno.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3jdzsvkqe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wwonqmsq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xmavnqlq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kgwxytqu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pgdtcqhq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wfgnxata.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3fkbvgxkj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3grddvsbs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3pdikhtrk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3vqhhupqk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qlvalwhs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3rbosfaom.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3qdkdbjjn.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3mlgqhzwh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3izdralnb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3lxvkjnlw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ndhpquuk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3mcjbgdky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3enwaapuh.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3mvtpdnob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avglxvec.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3zruiwcug.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3fcjbsehp.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jhsdihkb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3advqidfs.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3jevgaowe.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qadriczt.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3jnxsrzgw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qmcvugky.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xbhgnuxs.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3uqbkvski.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3klapllkr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3htxgduap.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxyiedfk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ifjeunbz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qlmuyvpo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3kokwnhvy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3qltfbxgr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tjicpgev.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3tusitohc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3fkojafmj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tfvnuoox.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3btirtnmw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ohagguot.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3epazssri.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3vbpvgmos.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dafowrom.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mpftvvdi.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ocjqakja.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3uernxgei.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojxuwtwz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckhwpcvo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovokqzss.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sjkcfwev.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gmenvdtq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bkrlkmxe.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ivrehooi.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3fvdmxcjq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ideqvelz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzebqjep.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3oaxbqbjf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqnttolu.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xdbaowby.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3qohjvnhi.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3rshzgcam.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3oevbxzsa.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3xwkyibrr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3pqibphss.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbvwasbo.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lddsvtwj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3momsqodw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ilpznqwk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3juprqksb.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ynrsnied.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3hjzpfyng.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ghenxjor.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3lwmjgvch.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3dbckbrlz.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dbvhczqb.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3belgjyxh.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3eczrjlhz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ylhjxmof.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3xtgipifz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hdimtwps.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ghvhbggu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3oaiqizam.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3bophdmlu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3hnhdgyja.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkadertb.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mszaxzen.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3hzfwfvbq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3hqtbstft.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3wauxlvsh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3tkzamqta.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3mjumokmw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3glbashzu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3uolrgxmm.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3smdjbowr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3axhbatwq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3wafpmlbw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3gswcgsog.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3piezbckz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3lgswpnst.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3afqcbmyw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pqqbbtal.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3znnyrgos.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3authkdei.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3yuijvgxq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3kdlbsemn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kdyuawzo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3rxgakveo.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3yelexqru.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3eixlxtco.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pdirlety.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufyofqzs.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3zznpntcr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlipdqdx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qsytmrhw.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ercidkvz.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqrjnodk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3hugofjwx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wyaktuph.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dqyvyxlp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihadglhw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3memxklyb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3itraavcl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xikjsxzx.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ufvfbohu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qmwprwae.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3shrskmcw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3sqjacpem.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hmrmzhls.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rwxzwleh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rjbfuofj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vxoabtxd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3lyyexcln.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3rhxzilhq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3txkzraui.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3eascxqek.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3etszxkwk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3pakearzd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3sixjilvc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ewjwdxmg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahrgzhxb.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3rmenfzvz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3phlnpdxk.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3dvjtgyil.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3boosldjo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3xptlpmdw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3xkjntyww.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3vuousggm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iokreqgk.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3jayeiqve.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3rnenpbte.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3wrcceyfp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3gxojdcgs.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3emzkjsrz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3jvhckdwq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3hbnajbwz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3byalltoe.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3gvirdgan.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ttegokrp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3dykawnqa.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ojwhpxzi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3tubiaeuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhhcgprd.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3uazvnsyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gpayrmns.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3bohtutsp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3kdcbujop.html


<!-- 参考信息 -->