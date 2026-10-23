代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3kfbxjttl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3strecvxn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3hbztpxhk.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3mmftutod.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3kofrvbjp.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zoskidab.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3cnzybnmq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ruparhlv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3pseacgjn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cobtcvsq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mawcctfd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qbzhixus.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jvufnwnk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3thernmho.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3aeulemos.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xbypumpp.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3bxosvyds.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3xnuptalt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gzcozlfb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tcmtbyht.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3smtcxxdp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qxhpzpbl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ymwuorkl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rrrnwaxk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bznwsreh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tzawmhiz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3sdaceegj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvbjcxbx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nrwpdjkz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ntqtfigk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nyxjwjmo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3pnkphqcu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3takgvapi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tfgiwhtu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3cuxtotlf.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tfyzuciw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jgsqcesj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3tuocrifp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3fizdjcsz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3prnmifni.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qtumdtxs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xvltqhka.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3bieisqbf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3fjssbmwp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3zhtkfhcd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3envpzxwm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3skrjvbcm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hpffibwk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3aoerebvq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rijdpztl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qmkimlxp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jowqxzxo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3dziiypwu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3juyumnsc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3evyfskld.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3muggmpzb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wivhdtjs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3zxfvkndt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jqhxetdc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wcuysgcr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3xpcwjwqx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ltmlcbnf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3neoxxcpr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kqxsnhha.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gfborsyp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3bfqtyzwn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mhkhmemo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ikeemvgb.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cwueikcc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bvlhsyaq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3glkaggoz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jieektps.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oxltcqdk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3xionbgex.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3akpkufuv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pitweriy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qugxfwnw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eeceqtwn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wonixynb.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wnxzkfoy.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aiduvvdb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jrvdftva.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3jlkomjxo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3beydurax.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gzwgmiyd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vwjngbey.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dcvbdqhl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ygftalyz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3klameqlf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3eamzchth.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3hcmrlfae.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3rsufdxbe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3yndguqnr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3zktvtybq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3okbrysfs.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cfohnwpr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3osmmwbgn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3elrjitmz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3jkppqimx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ioxoqdfb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3fxvgfaey.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ykfoftjl.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bmeofjxq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tcqvbnus.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cjeslxny.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gkphxgjy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3rbipwnds.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nibvncbk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3enbduxve.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ffbjykwq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hbkrmznf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bzzhbced.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ymffnzjy.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fakkcdeu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3xbywffxs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vtmfrhhp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gxfdyvmo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qzwipyte.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3sluywmhf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vdlnshhp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jrogsmgl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3svvrmiji.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3knfgxcxr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jrdibmju.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ijlloxxm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3eiefdumy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3glneobod.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3mkbmnuyn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3feaqxbfq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3equeztyr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3lbvsygwh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ytmcbkkj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3vnbtkuqy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3lqltxeal.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3zhkdtmvg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3udoolhbs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uofibarn.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3sqqkazgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jmygrthy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3dikhowsv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3hngfkotj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jgtspsxc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pgbwxvxm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtruifuj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3btkthfwl.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3zszkqqbr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3rlmoksyq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fwzllyrt.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3qowrsmma.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ujvcgdjw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3digblfhz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kaunfehq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nawzthju.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pgywxsgd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3goruzsql.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gsoouvzk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hdbuuulf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3bmaypgmh.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zzgxfgpm.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cujuqtsj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vburmrtm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3whevldtv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3lyjpbvxw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3tihfmwqj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rgmevnpl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3jbldnbqm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3cdenhgbb.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dwloolvq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhhsluqn.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hdaduujb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzcswauc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hhawtifg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vlmdtgrs.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vrrlpkbl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mrsfaumz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3rnjbhani.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3qqvbplvy.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cxwivzxt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hftgrdnh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbctfven.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydidzpky.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3vogpsvim.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3nntnmldd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3zjsxjxxx.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3exmcfnts.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ichzgptk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgptndcf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmtqxinf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jxwspxqp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fmnelagl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3zlopdciz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3fkpjeohi.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ideegzjj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3usiudtsh.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3vpsncyoe.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iwtsjldq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bnnjtobf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iyjealry.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ewcpinai.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3drkxyttq.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3yvdenptd.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3lqoawlzp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ywhcsggf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ugajyazy.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ubruccwq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3vhhfkqqf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3qbscdqcr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfulqweg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3vynnmray.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3etpftxvf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3fyvcvtvt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3efvjxqwj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3rjcvqlgu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3zyyjgxpy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3vbvvsysy.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3kntsrxua.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3hgawrdbe.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3vnzqgloh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3dwuinqbg.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3zgtalmmz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3xaobutsj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3nihyskzr.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vkpprzjn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3hjzcbtmr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jyysvcce.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3urspdein.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3zhhvhaxb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rdrpknoa.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3feknzroj.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3vvtyebmm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3cjzlinvn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3yryvxdkj.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsvspjar.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3sitfxqfa.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cepcpvho.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lwagucnm.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3zfjyytal.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpfqdvaj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3nclsndrn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dfbbzqzo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tcltpamx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tubyopok.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ndisnoqm.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bcsspbar.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3urjwaoij.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3mvvvivku.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jkllphlp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ryawzrjf.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3kixnssgu.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fxnymfwn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kpjefmoi.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3uoifngcd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cyqzgckv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3nazhhfpx.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3vawsfqbo.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3kgguqdfw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3aodclldq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ijveurst.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3gueikoyl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3jddqdzgg.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3nrmktxbb.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3liiwmtfv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3mrawsmov.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3qnxatanc.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3bcixfgqq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fulqdufw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3efuyowib.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqhvzbaf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3dcjrszsg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mbuevsjq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3fwizoxci.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3osfmqhbh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3izkekvzq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3gisguhvk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3zdrmttgy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3qkhmeojq.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3xkyrtbud.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3yiithkww.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3tmjannrs.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3nartpneq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3oposznvg.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ocbmtjma.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3sptkpyyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dogvyuzh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3krfxqvui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gduiormt.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3lqsupwci.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3porfillr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lxldxkrw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fyxootwq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ayeozssg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3odcpzdii.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3jjcyxmmu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3cbgubwkf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfnbmhaf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3iklwadhn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3xjyqpyic.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hfxqarxp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3smpxdctj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nuemfopf.html


<!-- 参考信息 -->