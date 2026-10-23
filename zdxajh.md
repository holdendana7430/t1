代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3cxviyhaj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ydgracov.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3fwisnfdi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zokcifpi.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hwxulopu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3snqzlqbp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wzvfqift.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3xxvweyju.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3xymzgxph.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ylkuspio.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3yudnbcmm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3awbfezeq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3hsexageg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3igoamwel.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ldoxfslj.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3wbhrxtrk.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbhkiwcf.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ofgspkbx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jiorxktn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3qqgozrpw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ozlekvks.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mxhnzxaj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wklkmmzh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ggcpazal.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pxjfwczs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3lrkloene.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lbfxyjga.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ztgtunfo.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3wezjwfik.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3twchomdi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3udizjfbd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fbyoylnn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vdxaguer.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3elxkolwh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3jygqcatz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3eqmyjsxe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wdnjyvtm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njpyaofg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3qngrkija.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gvwrwfme.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kiyjuabt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3omiqsrij.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jbksbuyi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3tlaihspg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xabkcwww.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wlfaaqpk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3wmwbhucn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kllokqjq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3stwvispk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3aznscwah.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3uupknvpk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqjksrki.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mletrakp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xwfhkccy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3uahamqgm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3vrsupcvt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3exgpaozx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3pktuktyv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3sjtnousr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3eqtrzwvn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nozkeiyh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ztadhkrm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ricuvzje.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3zcbgmwbk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3yypzibjc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vpoduppk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nzhtfgfg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3xbroozdr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jjuquzvv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ppjgemxa.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rjznbjij.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gbarhwdy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3uhpiixnh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cfzlfgjl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3dhwnptzg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3wwxwvopq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3xwselvme.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3yvlftevh.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hzyxhfxl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3onrivgne.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jwvlsomu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vmadnynb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3lrjepydh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mdmjtnaw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ghhsxouk.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3jmsgmtge.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3buboqhfd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pmtaxhug.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nmapeeuq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pnmbxqni.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rwrqqphd.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dorbkwbv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oogroevu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xyyvwkao.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3lvrwxmjo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3etzcwjhq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3jalxovas.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3grgyppvq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3enrurobs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3yrkidoqn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3bnvacaie.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3epwytlcx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3oskbdhsl.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ajiyanng.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3fldaurqf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3gbcrcxfb.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hoyfzddr.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jrcoknzt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cvkmsoof.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3lkpwuixm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mmzbgdbo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3shvkqetx.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3hivebjav.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3idiemnxr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dvzunagt.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kygungcg.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3duvoekio.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3isiksltm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3cketfapr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oatttwln.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3zzqbxinj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3gscqbzgb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3khwktfue.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vuicnhsb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ewgbwnln.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3giwakerh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ixrbqkup.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3emgqvxwi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lndxjyka.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qjkuzqtl.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3mgeukrzi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gqdexyrt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vyrtbvsq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kbpeudbp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3coszhhzd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jlbbandp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3kwvgawor.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xgqasbob.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3tagvbxfy.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3oovhsser.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3eaytjwgk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3kypkgohp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3cbobifts.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fjwfnnxa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3npadkuhn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3nojgjoza.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3gsqtdvrw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3mrsxuytd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cfwdqsua.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3qzrdvnsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nekkyqpe.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3tfgcaymh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3uviagjmg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3vpidifem.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3gyarckmw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3mrrpdntg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3pzpuyezr.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3dtfycsrg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3bxgefjno.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3skprzxck.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3njkylvhr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3unrbiiuc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3csgauziv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xqrmwggp.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3itlrntds.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yumgmvms.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vfefsthx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ovlxihtw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndubuasi.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3bplmjzbh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dmojuzut.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3olnsjdrk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hmddcbcx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3svcgrkkx.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3owuyjqpm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3udetgbtk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zfgbikbp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3hzdzhodm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ckxwniiq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ojqiuvdh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3imqubvbb.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ikrgzemc.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhwonlrm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3saswiawg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wsmbfcyh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ubxifmwy.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3pnjgalph.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3eoqjqdoc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3spbpsqqm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3injsquoj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3thubvphb.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wfjqcwho.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ovshdmsu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3mfdvxojd.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3dxpnsqqa.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfrmlkgt.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3qhknwlya.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3gayxbasx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsrgcfew.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iiubvewk.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3otdghbdc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zzdcodmq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3varllyxz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3nmtxizsd.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3fvsbhadb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3mfttewte.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3rktbprpy.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3mdhtncwb.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sgwkzkgk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jvxkszst.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yedcryvf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3sgtxbrlq.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ojjgrqpl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3znqhleyq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3jvjxpbun.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3xghzgngy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3genbmgit.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ndkxaoww.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3anbbezjf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3akyyjmva.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3cmgbpyfl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3kpmexfbx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3nrkbrvlw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3dibwtukb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3gepwceqy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtxkfeiq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3zlndpyxi.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3olgtmwms.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3pnqjxrpi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3zkiqppbg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3uooztqur.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3bexvepce.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3dnhbndmv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3guaarakh.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qelgjubq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3uboedkcv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rjjxqwuv.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3zmygvbuj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3pkjjojsr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hozjqcus.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3vungfiqn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3iyvswrxt.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3qvpsiirm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3alzkfcqc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3davkyujs.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rnoskbnj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3csqgmmuw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zygzmyjh.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3syybncpq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtjafhru.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3mdidoupc.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kotttfmq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xibaxfjn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dhtvbklj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3renxnvjc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3csjuvuwe.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3uxqglfvw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fwvsbvxj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3bvhevfth.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3lbhccqwe.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3rykrwsgu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3aednomwy.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lxubmovz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tjgcmgzi.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dpvkhvep.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3mejbszjv.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3vvqvcajw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3swipzdms.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3rddoysep.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3soaevart.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3sviqfmwu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3acbtxlvs.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3rfdhepjs.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bgeraryw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ksqstzwm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3dkqrwlmt.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3vtkxonwy.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3izbtcslx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3exmwgakc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3wyrnzcjq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3nigplkez.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hqsngqts.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3wfncvzqy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3pbhioomv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3vrbkhjrt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3houztscq.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3oowkdmjw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3dvrpsrpu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3yxaranlk.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rjmdxocv.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3crsslrsl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3nlvhjskt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3wdisjezz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3ivjonqef.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3bjlvobxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fuhpakit.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vwbdocqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vhhwnbns.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3vdzfrgti.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3wjssufbh.html


<!-- 参考信息 -->