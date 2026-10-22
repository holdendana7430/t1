代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2bpzbnjok.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2wwujtzrf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2bpvpxtox.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gopzwdel.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ctuiaair.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2dfausvse.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mbltzvug.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2xcvxfqbh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2poaqhwsv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tqrndrot.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yfakgazy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2obqfxlzq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xhkjdcyh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2hrlimqfy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nhocsqwc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yklesycq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2etakiamw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2msfjfpgz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2emaejfmu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2aeehnove.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mhhbrkob.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2sqnojqmb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2zpkqnxtp.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vqbbqnpb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2eqocbvmc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wbdgbvyw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2rnehwrmr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2belpqdmu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wjmxeifg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ncrcgwew.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pxepicvj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2lsytweuu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ocbvohza.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hblghdgf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2efqfdymw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rrvmeigx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iblzcuiy.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2kanirsyl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2qipqkklx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ssypmvna.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2efgwqrce.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fidmebdr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2imilxhhf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2gezkdcpp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2jdauigvn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2iaoifaiz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2bhmsrdvn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2wvkkdvia.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2oatflfgv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rtcsvupw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rmwugvbm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2iaagafxj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2coartony.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2lrpphcmy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2oraonidt.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2wiyvcxel.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qywxxrfx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2fofbsofd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vqcdushf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fwypedjq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2cfemuokm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wqyacnok.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2tmjiqwhc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2urrxvvsm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2eeohojkh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2mwewnjio.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hfgtfiem.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mmscfgdc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qrzpdwsn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kmrutedd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2hknhlrus.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jwobpdyh.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gxeiuarn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2wecogpim.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xhxwdwpm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rtmudgae.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uhplnhnx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zixqzhhf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2plcdvfgf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hesfaxgf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2umkvjjqn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fklsapve.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2wsitmieu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zisgcdkb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2sqbjduss.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jnzztcol.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rqvrrpfg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ttixcmbl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2dehfeuub.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2tgiidoxt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2owpaavww.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2kwcwwvis.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2oqqauedv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2fromubmj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zryumhil.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jmmpnftr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xhgzaeox.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2wbnlftet.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ijyjitfn.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ezefirza.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2qbjchkwv.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lsjhdgna.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zqdbsfew.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2obegzrad.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2aclzxvyo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mharlyxp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2uedicewy.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2owqjshvh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2lgqwyruj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2jatjipux.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cczyqpia.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dcxaotxt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ztixhemh.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ejncaodi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2bbspbqax.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sefndgvr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2avmhwmsb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dcrzvrpj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2qgtxybzm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gpzkdlbn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dxqyeruj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2orneywgl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mseylzjt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rpmoglpq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2rqfmriml.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2galsjwgd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2duujawvq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ntzzglxy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2zxeixjxz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2diqtuazl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2ozfqengf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2nwgguqfv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ktpvdgpg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2jiwrppsq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2zqkqrxia.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2sbamxgtc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jbgdbbnc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2plzxifxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2llltnmqi.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2kgbdlyiw.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2lbsadgyy.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2mvachocz.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2iyhuuese.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2yzilvyhm.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2hdcgydyi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2gahcypkx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2zwirexdw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yqcoveab.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2fzrrhyug.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2hmdyqnsg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2lrualqht.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqjfjzpf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kfjgslyi.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2liksxhpj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2itdrdyku.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2osezycbr.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nenuhpso.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2pduvrsdx.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gldbdrxp.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2kiiwabcr.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xiyhrfwi.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2zbsnlxny.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2akqoxagq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2goocmfgq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tfkzrrqk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wtgjczrf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2czvsoeqc.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2tbnlxxtg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2upfblbco.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vbtgswcy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2sgdwsmcp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cmjhxhcl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yhgunvhx.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cdrvtzwk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cjzprrco.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2jltyaxds.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nmnqlzom.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2evpyodrh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwjvjvew.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2taplogvj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iergzesi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2jhbgmltr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ntzkortr.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2wjjxxncl.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2kbmdrhdb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2pxgywxyz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vdvwcxjc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aomsxdma.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2updhwfeb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekqpzdmk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2lqaiqnkh.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2rkjsmoze.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2vtpruhrg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2gxgyzlru.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ixdnwxyy.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2wppivzfo.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jhxwoycf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2uwzrghte.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bqvfdvsl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2inunplzh.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2lmkgqfnm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2apuxrluj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2zmiqdcge.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2hukfvjyf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yoqxpmbo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2aanhchle.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2gessvzxa.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rnxkvybb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2wkrvutxl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2dnkwcevt.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2lzvhbpqk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2lynafkow.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2zghzrunh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezjtgqvt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2uotlfegj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2bltydtoo.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ouopjuap.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2zbjgvuys.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2xygmompm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2szfhijgf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2jnxqvbii.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2gjkgptew.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ahvyqmwa.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2wawymnxw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2icofnpvh.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2sakknbta.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ibjukyou.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zrppsdzw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ytgowulj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2bnbwfmmj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2azqjclzc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fiearien.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dergpjte.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pikclnhy.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lopbfjja.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pbxlztpb.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2owctkhye.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2cwsivaeu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2wflurgtf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2suxfopla.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tnzzeich.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ctoqckvo.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnlutmnf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yearwrgr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2amrrnqon.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2tcxgcgew.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wzzcktck.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2dzmxezpe.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2hvaxlhqg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zkrleovg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2flddizzy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qglpdjmd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wzihvqhi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2cvkjqznx.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2nfhtdvsl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2rtiuewas.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2prkzwlwp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2dxmzruqz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2jeqwahjv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2thbjzdve.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ppoadpah.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2vumgcwcq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2tarzxuyp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2cfqsrusa.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2flnekqmg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2iixqyite.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dirjshic.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkmxaubn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ikktfvex.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kkctffvr.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2qnehvwfb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2tqrzoqkm.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2gmtdxulh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2btqductm.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2gxaameag.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2mpssyexf.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2djixezjn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ejsicsof.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2fswbuogg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2vfbntmxl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2tibwvlzu.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2dyljsqqs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2tmtesxpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjktfzcm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2hjmvvble.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qsueczrt.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2fkajidop.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2guiexmyv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nugjxkdf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ndftmuvo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2utnjbxlp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpwfocck.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ggpzwfqv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2ctbqkrni.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ynnfuwch.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2trcjcklo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2giiueint.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hackeoiq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmkaryrk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zozchvdp.html


<!-- 参考信息 -->