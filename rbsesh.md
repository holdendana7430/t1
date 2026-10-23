代发 wailian999

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3sgskvskf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3oswqbayi.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3dgaibxcy.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3odoxytyu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3rmqskvwj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwvzyjfw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3laektltl.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3uakycmwe.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3wclnwiql.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3mztdrlos.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3yjudmziu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3iphlgiuh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3cntimwym.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hgkuwubw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zaociiwl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3viymxczv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pwwqvfug.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3diszmgey.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wddpygca.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ensojacz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3pocdzxnk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ticqjndj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yeyxpkpb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zusncmxe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ybyvecmd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ayknhatq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ilhxodur.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yyvdppkr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3izlgcmwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3buuducam.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3tmsxcfql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3spanjhff.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pmvypwsk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3gvctjufz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3isxijklq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3alineecp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dwkhovzw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3icwnongq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3eppveldl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xrvpbmle.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ieaudbcn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3lfkvhlhh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3knxxrhce.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtlqcepa.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmvsfvpl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wnjhvbla.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3uytpmokq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3jtzclnzm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3piohfgpu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3joawdyzx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3obdhfcfj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3fgtnflis.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hmgvbpdf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yqcuigjf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bisklifj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3geccyyuw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3gfwucmvk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3useiwthg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ndjtbdtm.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3hongzlyt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gfqpgrvd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3wftlbapt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lrkagfci.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3dxpvttzi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3hamgjrfu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3udrtwxzb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3lkklorkp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3oztdtiqh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3giexrtqm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ojdzpcdw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fckoukbr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zwbzjuqq.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yjgviznc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gjwubbsv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3veujqooz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xssbngad.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wqvtumbk.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3fqmytavj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ovdemmub.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xaoxzufh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nywsdvxx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3thdsklpx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pkwgfboc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ljqhiizq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xfjuvqqb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kaowcgth.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3sowvgwcs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3crninsia.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kvipdhat.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qjyjoahp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3nbmawryp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3lsxhwdnj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3cjskvubc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3uqpkntxy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3zodgtwtj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3zvufdakq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3uftxjwdr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3cybtoicp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3enyytgjx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3taiizodc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xhjittka.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xxbrhnmq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3lnjwvlsr.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3nspqtcap.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3oespziwn.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cvkhfiwz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3phsbamed.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3trnranud.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jjesgchy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kjrxtrro.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3eajmhjyx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ojedwqmr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3kqsblgqs.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3usixytza.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fypxuhor.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rxvchbwj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rbmtdepx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vvsjlggj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3rqrnezuo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tcxljbgt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3svqxldau.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3afobavav.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3zvkvzyky.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oagyfgju.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3oajoldsd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cxzpsgni.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rsnugyrz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ywbfuhdt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3zghmeldc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tbqnfgcg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3qbdfaupc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3xqwklaia.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3hoisjjwa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3aasmphpd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3iuwmxmzl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3kfxhuiqt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3kxmlexmr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3vqaitsfo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ageewiaz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3gelfbhqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gpcjkswp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3delzpcwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3egsdultt.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3lxeonior.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3nrmmkqcd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cijpvqon.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3utpjtguj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3swpwmqgi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gcsaqdmo.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3fdmtasbm.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3fowdpntp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tpajwlas.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3fdwlliua.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3tctisbpf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zusqbvnd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nivqudai.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jifcugkl.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukchnfue.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3igktpaoq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3abipcodo.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3phevmpgy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3bjqhnmka.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3fcpkvkgz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yxpkiqxw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yjdnhbrk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3eghhtwth.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3jkkamtou.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3rclqayvu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3oqfnkldj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3nfawntry.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3cilgtslg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3erbkfjef.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzxbxjmp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwgngelj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yxokfjeu.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zddmjdhg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3oawzlkcx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wasuzafx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3yfiknntu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3iywmpwgx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3kexpehes.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wcoyqhrv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3eylbgsac.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3itjchhuv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qjbciokm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3rvhxragw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3fepamfji.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3mludfeyr.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3omctlycd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3fobctidw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbakuboh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3frmepefp.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrffimgj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cpjprgqh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3jkpqnjcp.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3suzrpeym.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3uwofulod.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3pksgzzye.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3jtpxsqrz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3eyimlkra.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ihbslewl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ycmhvjxf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tgbxzftp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3unpdehfn.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3giqatuaq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3tcuphggg.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3njdwbanv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3idnqgmwr.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xwiaafsr.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3tcnwhvhq.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3bndxaxov.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3toeqavku.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ckdngeeo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3qledbnvb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtyjlxkm.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ewvrjpry.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3uaaobbtk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3avvhqtom.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3gwgttrtb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3wioeewbl.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywgjuizm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3kbihwwup.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3vicukhtl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3iipnvvmm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3pgjanite.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3czqjpyjg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tiuchkln.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3gidgyqwc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lwpasals.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3dofxafti.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3oekynnpl.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uoiwpqlo.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3bfbxlkwn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3anmjmvco.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3xtgfvvmw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dssqyzzw.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3cktfmafi.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iulajxtk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3enksibaz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mhepvvlz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3fgqipaoe.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3demlvfid.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yruihhsk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3fewiqgua.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmtrjakc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlzmbcnf.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yypeopjg.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gyfwcjkw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3eplmtlar.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3typkrohq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3boriuuny.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3flptolxl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3sdzjpmlh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ybtremym.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fcipfsgz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gcsfbldr.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lbafrnbm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3hfzhwzbt.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3uexawhyn.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ifyjsgji.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ixhnisqc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3byughioh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3yhxuuwhg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3xmrazbzd.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ysbzfxrt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3auywcpdv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3gkjtkoul.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3bufkulxr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ytfqnrvg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wqvwcyud.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3opsjrhiv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ghjuivsi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3viuiwqfv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bbcbaezd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3hnlvdyqx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ibznzsqb.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3vjitfbvm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rluwmzcy.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3yzbpurrk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3yrzicwuq.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3kojktjzy.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fqyzming.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dmrqhxzt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3dzafajiw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3bzljlcep.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3injfhfui.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3pnqlaeig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3faycydvp.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3vfpotund.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clyekfel.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3axmrqaug.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3btskfsnh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xzhazqle.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewohkphi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mnzbktkc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3yjrxmhis.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3jylvkhae.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3jldrddlh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3mhvyiuxw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3uvteawai.html


<!-- 参考信息 -->