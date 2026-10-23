代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3fjngkdpk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mscopqfp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3lkawrqfg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrjqerdj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3taxtxmno.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ntcykslb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ornrebem.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3skvhmbhf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3vxtkdjuz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3abtpnrls.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uxegejek.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qzqaonje.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jvmrzsxc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3mhiutogz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wksunhma.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3adjguzbh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3nbisealq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3njmsmrzl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ewcejyum.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gzlxzend.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ktnkjkme.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3frcyqjkh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3msmlbgrz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3atnjhogs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jlpwtbri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oajayjyv.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3cpjvvzof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zgxerfxc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3fcfeimhu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3pzgvzwdi.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mkjnhinn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3aiirxyql.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3sdigqyon.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sczrszar.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3pkhihuqg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jwalnoui.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xdivptuo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3jrklezxr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3lacyxyqs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiwtlhza.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vhodkzox.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gfhijlwn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ecjwvhfb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3jtilcdln.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3crndsley.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ahnkulkf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ehyzrrsa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3enlhbxoc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3btsncgde.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fncuppfn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kivrgtad.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3cldcbtmk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3aokomfmd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uzebajzx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mleqekvs.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3qpectbpt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3nfzprmhl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ramesbiu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qxnjbnnt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wqbcdyop.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3kpujaxvb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yctmmhih.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3jkrjjarc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3biucmanj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3phzpivcv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3dcgoatcq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3exnhtxla.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3umfzmcnb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oigpssaj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hsfsggat.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3uskjhhaz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sfdvgbue.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cevphgzq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3xmbdatkm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xozpzdht.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uxghsddq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pcpjnayn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fronokgf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nxqmneae.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lxcasijk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qxdapjyl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wkdypgkp.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3zuphfqmj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mkzvorwa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gcbptgph.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3uwncpdex.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ixfaepdl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3sdvulseq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3lxccagcm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3raaettsm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3hvftzivr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3rhbpixbx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3wwljybag.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3xnnojgdo.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qyitbslr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jakvdihr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3qjsvqyhr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3crrqnljc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3spethhfn.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ttolulig.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3bgjgarid.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qxmpgjwi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rhmhmevu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xovmgjuk.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kdaibwbo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gzzsmjdq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3swcvbfqt.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3endtbihf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3rpixsyme.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3nhukwsjq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jgyiyffs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lwnaouia.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3efvfseye.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yfutvzny.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3cqesjros.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fonzymjk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tficpmfy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ykofbvrg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3mxshljrb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rvkipwlt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lwgpwprm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rdnedvsn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hyftdeyr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hjwhyocu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3haixuauj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oblurjwq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3cpvzmuxr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3vhhlalyg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3kprtaxia.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3rxdjykph.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3modisnjh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3qrlkwnjx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3jzpfqmjz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3hneeftkq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3qdgxmetp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3xbcfsnhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bacfvddy.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3hhljrbqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jnfpzjqg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3wuqsfgzg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3rjunrdqr.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qpaxusct.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ixuqothl.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbggesky.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3slesooor.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ftzyuuie.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3diawdxho.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3imwsledr.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yofwuizf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3gsfdaaab.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3afskvpvf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebzxovyx.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nkqonwzw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wwfocyee.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3kpobgxch.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3tutuxhms.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wimgdzbk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3cniubgct.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vcqfflat.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vooyhdti.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ffsadrnx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3julaenod.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3fwgvhtoy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3wdmyuzpt.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3gfnqighe.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3lutkjrln.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3jbotzell.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jdxfktgs.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ewblgyka.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgfzahng.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kjoyxpub.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3leawimls.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dufdzdqk.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3erkpqqvh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qreoknlo.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3igllfhnt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3apceahfc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mtiuaxek.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gqvkdsno.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qiczdiuq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fqbeeevj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3loqgsugi.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3insygzer.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3xjqttiuk.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3yhuktjjx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3xqrzaale.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqpostqa.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqsgckbv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hicybxzi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3euxvvdcq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3bsrwksic.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3sfnojijb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3dkowmuao.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ykbvflcr.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3zrlikusa.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kmbgykxr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ulyofzqq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3irznspwu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lqptndsy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3qweiiysr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3wzatyaoy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3trxtvolk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3djymfoae.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3aghiducd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ixbtfnxy.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tlpoeats.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvkageub.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3lqikfifj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3miqejybb.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3qruisyqg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3wmixxvai.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3npsipdfj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3yjtplcjn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3olduclyw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3kckfhvqx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3hrvuyyeb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3icpgctmo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3hipocfeb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3wlveqzmt.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3aoiejbwn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3yziyqgne.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ukrrddnq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hnxaexil.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3jdedwhxq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vbsixtjq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3pfzjiqnw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3npqtyhve.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3imrmmhcq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3bitamcql.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3hsliiima.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3jgdwyaii.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vynqfhoo.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3sfvwqnty.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3nvcmglva.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffevnnvr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3aypvbgte.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3hptfvoos.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcelbvgl.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3tlvpfwtg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3fplyxfba.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ptobqcyp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3abhulrtw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcokmini.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wkjapzzu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wrgivgtk.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vjtnfscl.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ydxeclrz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3xhhpxijg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3xthylxje.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jklbigkw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gpndvbxh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zxmxfphm.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3juiobykm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3bymobggs.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3vjezciqj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3iibpenyh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3mavcrben.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3njculwfr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ykrmnjal.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3liujvecn.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3mgoabohn.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3dkahbchj.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3cbxnkyqc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3bxrcftmn.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3whovyzjk.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3hpzyxyjy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3hbxptfdg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3akhpnrfl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3dzoadtrj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uicklqgb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3eriplrxv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3czlqyico.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3opxyyyjg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vykynlgl.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3gdqoobco.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3rmqojwvn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3hslxutlv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3mvjeytxy.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ubzcrfnq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3nifedqkj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ynidnmjb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3zuyhauda.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3fblqklmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dpskcvgf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3smcighjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3whzntjsq.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3jlrskntz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3vgyaexzb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3oynqdxrr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkijvjqg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3uytjxwpn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ofamqhbq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ygnyutyc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3mcckgrcz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ticmeprl.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3uoycgrml.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3wvqyibik.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mtflwste.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxfzoufx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lttigyyt.html


<!-- 参考信息 -->