代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3besuilyq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fioawgci.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3onftswrg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3veuejtwi.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3uykfxkzw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3scnbvvnf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zvlsgkev.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3cdkusrsq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3dwiefbys.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rdpgemhe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bwtknsly.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nypvngod.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mwcculkt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3pnuqfkkq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lbviofbc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3umkhuqhw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3nadpwrkj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mbqzjzgs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yavoaiaa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zuhwzkci.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cqkloltq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xxgcqtql.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3xiwccntg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jaygikiw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ibugmddi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fshvxlzk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3qyxwziyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3crccblfj.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3cibirhsi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3suigmxpw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vzdiuwwu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3povtmwrh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ankwjbra.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bygqewku.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ovzllich.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aymuckxq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3edachrsz.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3rlknfvdq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3wrccqrya.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3glchiccj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3telxkwnb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3suvguwuh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dfnixkzn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ggaflsxd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ldvdhdyi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3nwmqzovz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3vouzcbtr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qksafpps.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fiammhqn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3llagzwvq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dfuwigwq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3rbhfkglj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3nwfstpud.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3tdjgubvr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3oyeroqrd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3trjawwrw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3pggiwhdn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3bitsjcwt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nevtaoam.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vpdczdqg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ccjsyjib.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ivzlirrj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ctefoang.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3woyrjixw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zrdwdgws.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3jgzueupd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lzoizuvv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3atnzmkhc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ctlcpsci.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wfqmjizm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3qssikhby.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lttbrvfe.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fgkrjhyz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3logtupnf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3askawwnt.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vbvinjks.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wgeawysg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kihaczsw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ocokzurs.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hkooilbv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jtfsmegd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pjvxhzxx.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3mwqcjngh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gsjuznzv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lkeumkql.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vearwgrt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xfsbovgy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3agddtyqo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3nvitwqeq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3cdamldhn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ajmlpdzw.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3tajwcesa.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3dwrrzprf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ufoslupl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3euybnmdz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pfgccpda.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ykpjmtdk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cuspnegi.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3zxzcniqm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eflllbpw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3enqnswvv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zcdmguvr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jycozzuf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wbdspsqo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ssglzsek.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gqgcqtxo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zozkhtfv.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dvvdzjcz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3datnunpy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3pcjxfzsr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nujhhifm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lkipamcg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ezljvzbh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tnmgxxjg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3krhkqnlf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3emshrxfi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mwwnqghj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xemcstzl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3lhugkgxa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yskowzvo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mgsbxlto.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nxikwlcy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pkjnlbkx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nbiinukj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3fodbiaeq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tfptdbwg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3abygprkg.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3xjmntrhs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3cqvuuyxk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3nubarfkv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3sljwkpyj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3bqgwjmcf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3mwbfwyvk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3vevstabj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3klffhnfp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3mtcjxxfc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zfcxjxpk.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3sspahneg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ifsmgjmd.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3cnosbpvl.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3wgwyngho.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mpwfokig.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qwzytzyz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3jddhcjub.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3cscqntzu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3iuenbegs.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3frpqddoj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xoxbvasw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ykpfyexo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3awizsuvm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3jnagttpa.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvwklnnt.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftdvhzhk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uabmosiz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3hxghqcue.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xdxzotbf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ibdugjze.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ijknqmju.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3cbslgnth.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ztvzasap.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cqjmhfyv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3blrtkrnu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3wxodilzu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3lkayqcbr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hfkgzsfi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dcybvjfh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ejenosnh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jrgosspc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bovgirzd.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qebykcqw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aaykzbvm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjatonps.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dhhwiggu.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tpomwmkv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3dpupvcdi.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3zbbaepqn.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3glmffpyn.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ardfzusx.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jnfghuwg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3voumxljp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3usutzanw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3iosycqcv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3jyttpsbs.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pysweezv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ykplzjrj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3olsdhboi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgtgpzyl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kxosbhfw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3edsektrx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ovsigerq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3uyxbdffh.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3zkdxgtsf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ttsaeipg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3xhsyhmnb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3csupufic.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iwgiufri.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qdknygnx.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tpyafgdk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vtaehgnn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3itoucdkv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3mwayonhn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mllnbxjv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3jysbqjsu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3anzuasju.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3aekcedim.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmnfmjep.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcytzlur.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3wtynbldd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3lnfxjhwl.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3qrkitsdo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3okcuhibd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3yhhbhxup.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3aknskrai.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hrrchesu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3fjqxfhem.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3swmpilmi.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zummrbra.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3cmddzoud.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3vuvvbtau.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3cjbckbrq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ahoxyttl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3lhmfwsou.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qqvkwmck.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ebdzfigf.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yoksyakn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3napjzvjj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3smjuzehj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mpdhhkzj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3xvihbrwr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3sspxkulf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3jyedvzlj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3skvbbqvz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vgbubajl.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zflrxjer.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugrpuezd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rqhspozy.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3efdsysyh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3xbufkwnp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3yrnyauil.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3olwijcsp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wyfdxfbv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uupzjxds.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hbxavtaf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kceppsbo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3atjzgner.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mmnwuzvx.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3kfnjcxxe.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3bmsgfmwb.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3qdjlmwrt.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ucttusee.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jeezzejq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3biumjkvj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ilqxukrh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3phshjgfe.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ysjxxhaa.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3hzembgcd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qzqhpgkm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3eadehgts.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3woqcwyer.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ffbnjagb.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3vztpllrq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jfulatqw.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3vvkeupqz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3hfrczuvr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3gyqthvpx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3yddqyakt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3cnzcpama.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3qyikuhzj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3yjxavrei.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3dfowyywk.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3hqqfgzic.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3dvxhsriw.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ekauuemo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qdnkdfux.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3sevbjzih.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ybeyohob.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3hqysssms.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ghixkfne.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rmftctdm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3thlfnwsn.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3dqmlqbyi.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3xpjcmiba.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xinmvgbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wxppwdje.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3cjaznavl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vftwpjod.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3bynlikqt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3exzwrbwe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3sikhcwkb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwukiqap.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3iabuwjwq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbukhidi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3gjldlhrd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3poxdhzex.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3jdgbjnhq.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3uaoqngdl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3czldinsd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3clyzvmzk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rqhhhift.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gdochvpb.html


<!-- 参考信息 -->