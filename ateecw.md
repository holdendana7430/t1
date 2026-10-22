代发 wailian999

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmszuzpv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ynozfuwh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2jxgmgess.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2gmybwdss.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2vainrclb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hmlrazqu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yadhjtdh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vzrpenae.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yhnqprun.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2msaezser.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bixeajab.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qnkszraz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ghidkuak.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2komghlle.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jkrpfqrg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zgphkthr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zflhfhgz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rvrwhrnt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2xrkcldbe.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2digpvsom.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xjpqifsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ypaqrerr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2mnxxzezo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wrnwkfjp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2aatebdne.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2nxzxiypw.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yijozbbo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2qdhtpeul.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ptchjhfr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ggyxxgux.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2agwilcks.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ggmmnnho.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2imuqxvji.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2igaqeojl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2jsgbwzyo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2seqkgabc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gduxmvpn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2irjibsbq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2fqitrpsq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2mxlfumgv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2uqmqifjo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2djqnpsgv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2gwnvchbr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mvjyivwv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2owbbdsjl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xekdnmcn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mmyzaayu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vivswuen.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2obyzxylj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kwbjuota.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nvpvsuzt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2zxiqhimg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2axhfteum.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2iqsgcrty.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lqzvzydj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hvzkolmu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2gzrhthbp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jqixzteh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2qtjebwhn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2oebnsewa.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ytnxotkr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2gdtguffi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jbwmkpjt.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jknbmzsl.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wtnznspl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kfbfifkg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2dacpkbcb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ahtiumlg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fxcihraf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2rbtoafnr.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qmlkkywt.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wkjoalfb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2icetehnl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wpqjjgcj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jlhzxjym.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rcejseig.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ehwmrhzo.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wpqbqtap.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2xblqviuf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nknorzgi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2tdwsxbvd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rbwflkbf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wazjcpdl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2fmscusbs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2vpqwbquv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2onwibxty.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2smemwbcz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2rnvjjhgs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2fgkmvvki.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtcdvdrp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qdczzhej.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2eeiehcbh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wbrvqrxt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cnqxzoko.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ligfnadt.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xyvjhart.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2eyctvdch.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fpzlpgzy.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wqcwmzdc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hwvbpnzd.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hmireusv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wnpsxflz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ljlziqex.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uevzapoc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2zbmhkyab.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ufybgoms.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nwwrekyh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ojdudpbh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sbtfowcs.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2asixbzpd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2zlnkfhba.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kqkkrjyp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xtkicwlq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nkqfhdhl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2nwyvzfix.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2syspdbqq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gndcvbud.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2eaiyvqbr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xhjalehv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2opkqagqg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2nphhgxqm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mcytprrb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2agfbckum.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2yjkidgnm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2zftgbqjl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2trlzbzrz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2fnyjhzwp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2hzqpltur.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2xhxqxvec.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2eozcvsda.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2vxzbcvdc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ejqntege.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evljwytm.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2kitonlak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uvlrjbcb.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2stlcnsdx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2idgamkjb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2tpfxngfd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2spbmfvms.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2chkocxou.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2hlgdaeuq.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2pwcrssgm.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2fabkvsuy.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ktjxoquj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2herloekf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2xywlvvou.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqqhttcj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yaafbkws.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2oisysvha.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2omcnlzof.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2jenvnqbe.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lmmiohzy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbnsutdx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2oiihqjsb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2epgfzrhw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ledttvai.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2twsfdmux.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2luryfscl.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2hnejbudi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ujspzxlb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2cwfcwfvq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2atihkbpb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2amtuajxz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zbsgzmsa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2htyxaycs.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uotjnguj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqnwjlol.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nohwvccw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2aidpiadv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xafmwlbj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vkpdrntc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2sghopgsg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2greodmqz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aseoyidu.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qwtbmvig.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2txxwtanp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2whknickz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2wjikkvsu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2glaesyph.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2cmxctxsm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2iklqawbk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2siszwpxp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2albcvfzy.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dwaumehw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mwfuvzau.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbsoeqzf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2mntvdrso.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2swjlwrde.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ysvioduo.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ojuvvtmn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2oqczwook.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2mgaaizxv.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ldcraqql.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ghsqhgqd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mwxesebh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2hydyybwk.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2wrnzqwaw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wuzhdbth.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2xktnbdbe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2acbicyse.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xyggzjpy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2lcptxsrm.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2zrhksphx.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hicfngzr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2pgnkbnhq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2bnlzejkz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2zlcjauza.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ydzkkerl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2vorjufle.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2mqtqnqks.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2rmfiofvq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2icmafhze.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2aqrfgexx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2onklvcuj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2exbhcuis.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqxkqjcc.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2gisijvcf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2dfaobano.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uvuqjedc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ahvqswpc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pdafjiul.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ljdzkbzp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2jlltkric.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dkjwdsmq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2jjqbmlha.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ehtaewxs.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2gzcnbdge.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gholywly.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2njhlewlq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcbeudrs.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wjlcyogc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2optmywgp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2dsjgzxjl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwaurdrn.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2eoeddbhy.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2yzkhcezy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qorramtj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkrcnyvo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uwvbhasx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mbgmiiry.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vzkjjopw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2axqxwyxt.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ppwhnekg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2pmoialeb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2smtphzcn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mjfmaluj.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uguqdszl.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vcrbjxkz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zdjwmkeh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2puqubvrx.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2uskkbdfd.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2cilutsrt.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2uqgxunpx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2eqtxexhl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2mbhsrvyi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2qnfhgiwl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2lrtszofa.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2wdzlthnq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2puthhotq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2cjvzevod.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2zvsvyvab.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2hepkvzkk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2aijdyxcg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ryxnxdfd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2bqvkctpy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ocpltsij.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2feawyxmy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2fpsihcnc.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2sqohvvhr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qfymftxq.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2kclrlqmh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2eyxbdity.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2tpvciyki.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qdnjeudc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qcyqaywy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2zyyodorb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2psygdhyq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2voxlywnn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2eminhqsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axgvnude.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2lycgeqdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2htxutudf.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2gxpagnrp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2feiqpfiu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2eqovomgf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gquuouib.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2wiozvkky.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2uetyijhu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2oxfcoxxl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2uuaexayc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2pjrhehsr.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2gtotvomi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2twzctmsr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wktlxrmx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqijsigd.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rheqlvpz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvnuvycr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2cbztnsyw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2zixfdafs.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxngsjxf.html


<!-- 参考信息 -->