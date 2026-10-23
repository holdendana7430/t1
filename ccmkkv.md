代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3yyqehffo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dgjqirad.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3juuvulgl.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zvjhjfaa.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3lcztlutj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3mfyolwbr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gorvumgt.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ihcjqmpq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ujvxpmaj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iapgznqz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hlnnvgsf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jarywujo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3awauzpdd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3dksxlkbb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rxnzukza.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vakuyuho.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3xbinrlgs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cxxaemrh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3etrqhohw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zjmpldoi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gyfslawc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xrhaxtmb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3nzeqqzan.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hfkqydqz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3aydhfdsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3diypmkoo.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3fxydabuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3srhnyxsh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3hsadbvep.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3wcmtrgim.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cgheqrki.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3tytezsrx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3khvygjks.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jkeflnjz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3oompvkoy.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qarfpfwj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fmcqrmbn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3gcauqglz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3irsiitph.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3qsdvxpxt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3umbzpgii.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mlwebzoi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xtujbaok.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3riwazubg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3joxvvlxy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3gsigesvm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3pjjgllgu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cxujonpy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3refxznbi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fpzscyay.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3skejsxji.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3iuqlneay.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3kkilgjgc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3vvorwfqh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lzkvyzod.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3euijahdh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3fgdcjvca.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3lafdqohf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3nmbgpyki.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qynvlvrj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ueqbkyuf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3szfotmkt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3xznogafo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3zlceaqol.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ifesgzjm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3cwihzxnd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qucusoyg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lxjpgxlw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ftqlhwja.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3innmtmhb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3evsncdnp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bjvxmrsh.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sjrazoig.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3hazyxeze.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbqpvplq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yinthqfz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3irutknnd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tvgdiqwz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rmdvbvwf.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pcjqknkf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cgkjwduk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pnismwuz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3sbbqhfhv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vridxkyp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3fpvqnxqi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ayntpzno.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vlmjyoyq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3tpafhfva.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3kazvjnmo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3fzdojiyq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ugrzilwv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3rsbvlowa.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3fmeoxhdm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ensewwzs.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3gmjhhfbb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tfrpgpkn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lqzhpxtj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rqlslbso.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yljfjzhb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qonrkrym.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3dtqtjcdw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3allqybno.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dvtjeiyv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hhaadelq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3knkqbige.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3eacijabw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3pqhsjymc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eczonokl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3fvhbdmtw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ntrhuxhx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tmhafyrt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mftgzsil.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tqbzvwae.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zftnlpcz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3zufqzcoj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3frbeqlha.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3urroscar.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tuwvytnu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3mzxfvycc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fgnbhmgl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3xzkhmkac.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wviifcte.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kmwyddpe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3apdqmbaz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ybzvsucx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zggziivq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ldgrzsel.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3wyjhejut.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3tcvvgwna.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3lwrmesad.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3fmppjqrq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ookabrlj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3vcodrigd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3crgwkrrj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3pvqsiuos.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3lsnbxnaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ojurndhc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3qfftxpmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3joapuika.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3hitkogpo.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3knivbczm.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3btwqfwun.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rgsbogyk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3zopcyisn.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hutdmndf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3eunkqpuz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3boadndhr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3cxdmhdvk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ogwnulef.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3pktpkfyp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cylhercu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ebcdgeey.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3vssxesss.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3slrpabim.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3khyfqxkf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3udpgrssg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bfnnkdfg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3iikpeksk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3cvjyvqsh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cvrlhrob.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ljpcajhu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nyrcosjy.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3glgoyqpl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3hfdzlpnu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gxhxkxat.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3fjpjetim.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3loaxeily.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ktagokrg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dchvsexv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ptseuoat.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymapecgl.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gagmpvnn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3krfkvmtu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3wzqgiouw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wjpquodz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3emxcczlj.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ithefkex.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xqlstrhr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3blujjyrp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uwchehbu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cgdpcrri.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3tjnpgvmq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3rfuzfqgs.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jgjftink.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3tzwgeibq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3zytlhxzp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yaqphtnn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3eukttsnk.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uwlwazig.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mycyewag.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3cnozdctw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3vzxdnnvb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3psetnjpk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3jccbwwii.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3wdshmusp.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dsenibez.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kxqsmxwz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mxscylzp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bxidqpdu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3mojkfxxt.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3gbbqlxef.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mooatuaf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3hxuxmkgd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3tkddimag.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3fuiknuly.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3clnzetbh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3yondwcym.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3jgpzcdda.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3vvfrhnsd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3rjvmyddv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3fggqilrg.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3xrleyjhv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ojzheihn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygmnvxqy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3kqnwbhdp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3smdkjqtc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3mjooomfp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3tmuqoudy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3fbxwgkbj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3lwguusje.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3nzkajdsw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3cbzwpweg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pvrfftud.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3kkejijrl.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wsszjhjn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3cdcampfl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ongzdbpd.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bcqdyyse.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3pebkgszp.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3uvimfsli.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3kvwjlbdf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpoearia.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3flzvcepe.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydnwpqvg.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3niprgbwx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tgizixdw.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ryhxpieo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvbtwbkz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wqlxjrel.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3expppbzf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ddszwhda.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wqmwdjih.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgjljdjl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hfewpuxk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hnreqflz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3lbwojfkb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3boppxqai.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3imqixoeo.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3zlsxcpjc.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pnwhcgsp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3frdvieez.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sgvdeiik.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ehfmbxtf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3qwbtgbpg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3upswplcg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3wfyactqj.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3ohesxavq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3qcxkgsft.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3cnyulhxs.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3anxevsuo.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3jkpafylr.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gyvwipqc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3dtwuwoif.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3euqladbc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3jnpsqkvn.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qbnnyjah.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3cnjobmyw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfoiebud.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3gdptfgmj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zcnymdye.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3qoobnofg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3vcnvtcct.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ggynwobj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ahgaodju.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3zxyvbqdw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3sqpocneg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3msrfddrb.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kmdofgbb.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ezrzfkhp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3kbwxfebe.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3xokgkudo.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3vgepgarp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3gytatzwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tecqmbxc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ldtmepek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qquhqahd.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3myozxykk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3hkbuclfl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ygwlyyuk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3czrqvtub.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnprxkce.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3tnovniju.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3wizhhkir.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3xdhatjew.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvdaikvv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3emflmbzu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3tucnyjcl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rtdkhcbs.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xygxlpyv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vrhaqrxx.html


<!-- 参考信息 -->