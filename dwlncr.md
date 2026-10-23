代发 wailian999

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3urhulxvl.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3yvtafskg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3zqjmirub.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3xqciiwuz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3uzaxwjzm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yrmwmsut.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjezxpva.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yviohafy.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3pmkjdfvl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3vjnhamhl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcupftzl.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3zibwpkyw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3kkynoxbp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qkfdgrps.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nqedyskc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3whvdqiew.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3niqrecer.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3awpdvxkq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vyscihfz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gcfkwsie.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3bbbrkmah.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bawpalpf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zilquycd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xsbkbuvy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3labpmhlm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xpstuscv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3fbggmxtv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rgcmeefr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qdjuxcsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqyoueqx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ihnzikyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nclfvzti.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3veqbialv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3uollmfih.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zkscvjiy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3sarxdjhy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jtyvhmtj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zexqvtar.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3tgllfgyk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cajufkmw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cqbbbffj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3trplsemg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3kcktzioe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mukyncdt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmnujjnj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3izlpcwuf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dwikhixq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3svzgbrcu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3vqaaxria.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3rnxqpqqh.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3iynlhzqo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ogabhdfv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3tqynjkdx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3grddpyyd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kydrzefz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xqtstwjb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3gnbnowal.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3klcdizms.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gspyzovr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3vvdnmdew.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ohqxrryv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3mhxsdzir.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sfdpnjzm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zzvjggnq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3tnwkxzcg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zaoeqyih.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3fdewsybm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3slkzcvyt.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3aucjryvw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3hcnhunli.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mvcmhcjs.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vjldxsuw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bkhakqhc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3apyclemw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3auktipsn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jlghwckz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lzkjlqjf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3czekyphv.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mlpsfrnj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xcxbylex.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3slxhrejj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3swvvkevr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vczeuuom.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xgvvwofd.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kbenemok.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ewhjmlgu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3wpewcanc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xdktkfua.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3kawybusl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mbuorhtb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3icbtjkrc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3omajygds.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3hzqjhxqv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3kxliwzjh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3aenthsnq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3wgswrxyd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3tirofqwu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3atdzfrgs.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qnvarjzp.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dowlxfyd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3scbfycuj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qhijdddf.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3mznkpllr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kaieaacy.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3krxojouk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ietjhltm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tmhrqfvc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qchjoxzc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jfcrtgde.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rnizpzpn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3djtrjvtv.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3marxhtgz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3mbgjtooh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3bftqrhqn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pvajhacu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3btqewhsf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3idrmgepf.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xuplsypl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3caczsmya.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3txloqzwd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3onkpiqgf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ylfcxhel.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3buajpkwz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tchwpqqr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ugbqagks.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tjiffxbw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pmccbfid.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3asmiumnm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ohqwmbeh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rmnpruaw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3zpwlobhf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3kqmtovij.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3hzbbqqey.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3tqqdbluk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3mknhevgr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3kcrvakpl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3mqpjsioz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3jxcffgte.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3vtdwuyab.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3phcwgrjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqstggsw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3xarrjnsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xduawgob.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3kxiztvne.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3xdvrceeh.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3hcxaavha.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ubngyhvh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ozlzpdlx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3subbooqf.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3vtyqfkqg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3mlansdup.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vftqzegf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3jyowaonh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3oylpcehb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3cesrbhay.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gqsfmbgt.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3phyevxjk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmevsuyv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3xntvvfea.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jgaxnwol.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrsrgejh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3lymnltvf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3tnhyqsth.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3oughbxse.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cvxqsxgk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nzwdaexe.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3rmzoujvi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3wjgklddf.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ozkpetnl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3zhlelwjj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3qgoofzgt.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qcendlma.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuhinsnk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gyupbymg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogkeatab.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfrkyrmf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3frjszpoi.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3iqdjylhu.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ojaaialb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ksfwtcbf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3gkdpotpa.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vptcwbwi.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkspchgq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nqdemuec.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mcdzsnwz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3vstgzqic.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qrdrkqdy.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ljkmegwu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3qdlcguae.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3lfsokyxx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ffzmyzev.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ymiwhbwo.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pylzjpix.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3igotqfvv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3khzuvorr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3rrnxdwdg.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3srvqhows.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3oybryfxs.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3axouvyxs.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lsvehvvm.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ohedkeph.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hrxhybxv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xwddhzjf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3bbqjkzxl.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3viioxpen.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sbsonshb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ubqsoobp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3znkgzbds.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3cutobwjd.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjojcedu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zkvqwqpa.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqzqypmo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3daktuhow.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3njgkyrfu.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xbpffwhi.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3htomkowr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3nrcacjsb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdxgesiv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3kreufdut.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3aeqejdqo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ceaempcx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3xdbursaf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3lkjmkdmw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrlnyzoh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3mgefabmg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3naoppnks.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vsfklywu.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3lbsfoyfq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ajhfujhk.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3fcoloeeu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3cjuykrco.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3soglueed.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3mgwjbbzg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3edsojkmv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3qfubkump.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bandxrpl.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooqvrjrc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbnlegpx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3llduknhs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3frgnfxjc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3rthirpai.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3mmzdguvq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3dicnqhlp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3tqkucdli.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztcgxexw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wsuhbnri.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvhddvzg.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rovgcwao.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lhlznwdo.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3phregjio.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jkxzkifk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3cumzwvei.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3iagexanp.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3bnlpijfs.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3eqefvvql.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dmhqxapi.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3istzguaz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3lcboatas.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3cykilbro.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3aimncrxq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ctaaagps.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3wpqggduu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3yitgiyva.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3clvdgfdh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3hsdcepkf.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ysuvmygz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3yishzvnb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3bwjnfdzt.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3tjbhhutk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rwgvdgoj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3gsmvxouw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3cgofwwxl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ezxshlmt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ukuyisyq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3hotryavt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3cfrotqai.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3lfchgvlb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ftoobhwi.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3gbhidlie.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3lzbffymn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3qrkorcma.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nfgvvxnt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3njdszqst.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3fptknoih.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3kmyyzazo.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3iucjzgff.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3rlnkkoot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3onacprqf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3xxxqmjnu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dibimkgv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3stgjvkqc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3swmsjhqu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3exluarpv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3luovsxtb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3odjngsgk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3nqlwjeqh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3srfvnfkf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3jckxrscj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ugsirrwr.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3pzdihryh.html


<!-- 参考信息 -->