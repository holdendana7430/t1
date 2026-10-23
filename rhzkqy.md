代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pryqpvds.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3apvlcnzt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gttgnylk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3iglpgtmz.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3fdilozmx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fzngovwu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hpgdvvfn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3etdvwaoj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3plgqtigw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3rmznydux.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3gtfixjjn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3izrnuuga.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3cncgzbzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3muiawjik.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3qsjmknsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fjsvzmah.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3onowtscv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3vazdfhli.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ztlqfncs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3sjatosyj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yyugwssv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uthybpdb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3snkunejp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sgleernl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aekgomhf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3jjyhuozc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3tsfbnuai.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3skizjjwl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cdrbhaoj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3bqjenwug.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lfcpdlja.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3sfgoqigv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3fmuebhqk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3fhsatbnu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3vdnmdubv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qeayzshg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3frjamjup.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tfppuote.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nwfiugdq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fghdjvkc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3faymzwsm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ctkpnqfx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vebzepum.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3vxtjwznn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xvjiqlvs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3zewoxjsw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cixafhka.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lycwqdbn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3leqtzesd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tmjsjymo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3zykiqtcw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3lcsovixh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ignnglkr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3meflbrhx.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3epikleta.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3unmibuak.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qqdborzu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rpzqohee.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3clahdcfv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vehwtwgt.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hhktjfmj.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3uckujhxv.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3osocedau.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3srdgcnoh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3suqgyqag.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jdzgbfld.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kzjfowsq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3skzhdynf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ckogbohp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qrdkuqlm.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3rlkkortk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3pnzzobhb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3xjvsifpt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3woohnkhz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bpdefnag.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3aezcorcq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3dxrjtjif.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3oyricdlt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3manlhxee.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3loqdfxno.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3mfrbhxty.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ggcfloet.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qhwkcoxz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yxycuuwr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zbmtvarj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3shojhmbx.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3bhdpdgnw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3wbvhxtih.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3mwjjgidk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3drtgiore.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3imkohnxs.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rvhfxwdb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3mambqgxv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3byduwjld.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3mjoifyhb.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jrooinjr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3xkcfvlzq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3qcgutakx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3drllacad.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ayaqswrp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eocjeyzf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ehezjtsq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3mjcsqkga.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pfhzwxis.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3egyzhcdn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3geohvnep.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3lmczrdfj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lktpirqx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bwgoqinq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bpqdjmru.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ggmooyvt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kzrkziqu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3zifhbjit.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tchdpynj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3vfjqausf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ruwshmpb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ongbbwir.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3hotpgyzc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3piiezswp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zqwtoovy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3dbekygic.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3vovryqox.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3yitvallk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3wqigsruk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nluoegrq.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3qbnsijfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ucolwgnr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3jbvzprff.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3llmxdalv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3hxrwbkcb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sxoieofj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3kcchpcdx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iswnbgjj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3bkxnwmed.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3wqsnnxgu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pfeuihzv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tnpijpqz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3paqqrnll.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3akchbnnc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjmcfzod.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gcstobyj.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3daxsapjp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3bjhxinao.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nwkzyrxj.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjipvpqn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3pqrwhlnh.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ohcclpwn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lhilpqmg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tupvjsng.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lhuwghpw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3dgamtqlb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3rzbxnzuz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3qhedqzht.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xwazvedu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3exfzordk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3zqdesezg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3trfuknod.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihyatbip.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ipsmaqun.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3djrnbsvn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3byjtyitm.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3yvbabnge.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jtwtgnbu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3tmbxvbvj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3snsztzii.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vadoiyar.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hurgdcut.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cybdehnw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vffnrekt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3lwomjwnp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wenuyats.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oneevfhg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3yitmceov.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3nlkymgkc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzbyxjjp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3knwglmne.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ldfvepsn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dzjtywrx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3nhsabhxx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3xdykmwoq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3euczmfoc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3dlmdbgct.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3bjhffrst.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ohlnmioc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dhdoutcz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rldugvks.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iylkbtcs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3qdbtkxjh.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3rkpdxnxo.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3qqxdyesp.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3kzdxkdbr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hkkoxcnw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3wruafswz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ootqxxxx.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3qbgbmvoi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uacdhdct.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3onmcjsas.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3tekjyijw.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqjljzfv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3xomxpncb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3nubsqoqp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzowyjdv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qzklbbri.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3thkaklnj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bzdaqbeb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3janthrzu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3muauhokd.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3tfdytlrv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3fwekklrs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3havjinis.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ldmclgpb.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3rrfpcsbd.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cmdtcmal.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3demwzrxk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ahijjsqa.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kdpltril.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3fphprbjr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3uivdlroq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ktxwihwx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3voumfyid.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3gssjvxwz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ncoeyskd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypprbsmb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hccbjsvw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3urwlksxn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3rsngpops.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3fvuqqlnp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vinuggut.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vecxsvwn.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwwtzrxy.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttxbxhvc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gxswxcab.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bssfoqgp.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cjioqsiq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wpywozlh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3sucufgcn.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ixeglaet.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tfkjcihv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zxbsefwa.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sgdllvfr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wbsbymxe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3eukrizfg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3fvgdfcng.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3mygzovpy.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3nmlvagsv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3uaqhnazb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3qxfbujjz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3xotpojlk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3fuachtcy.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tawvxtcw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3gcmtomyo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3skveiakp.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3plliujew.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xtlnrngh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3puibmsyp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqrjodpm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3pduqurej.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3lvpsfrnd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3eozmaxkb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3tsrzrkvg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3qgafefod.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lhypqddu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3wibpiloz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3itjpccgx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ujdebrui.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qvsamowo.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3dlejzhkh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3dwbjztus.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3tadtjmpj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3lwdckigp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3gkuvfhwh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cqdfkwrj.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3wwbhszzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3honljxbs.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3latwwlmp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ynxbxgpc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3hzhkykkt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3lkhuziup.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbnzkhzd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3cbqjqwye.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3egtjtdds.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3svufgfwl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3pjfihviq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3zjhnvorp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3paymijyz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dfoenngz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ngrzcfte.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nmflzpfz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wcemtmnv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3wrdxxwac.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3hikimujq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qjxvroci.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3pcjtgebb.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3omsooasq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cbjrsvij.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ncqsqjxc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ollnxfbq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lbibaxnb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3owotsqxb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3gceglrdh.html


<!-- 参考信息 -->