代发 wailian999

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ctvjrhse.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2rxxzxqum.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2dhvduoiw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2eicitpxd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2uxodgpnd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2lxohgtck.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2qysujcbw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2beqmhaow.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2vigvppuk.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2xwncmiyp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ghlafbot.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ayglrxja.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2uoshfblp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wdduodri.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sjdgaghx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mwferyat.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hotinstd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2xuaiepiu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nmvqbedm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2krvcqruq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2oblmfhsw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2avkuigky.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gkmyrrco.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qpbashyt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mbnjcvtm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2qkervfnm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2xpzsogoe.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nxoibmdk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2eqbpewzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nvttkbtd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2gqteiraa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmztvlqe.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qjamesdn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2cuukhwvf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2plqhpcqy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2wpspplyn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tqtqexda.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tlrjtdom.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2nnvoctog.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ynyuwxhi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cppazigs.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2xallwtgl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2gzwaojzw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gntpdttw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eiqorybj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zkltokyp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zzhprozh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2llhivxjb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2nhbrpiyy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2peqeflqn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2dikpyhvi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2eostesbd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pzukajxl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ivmpluei.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2keznsafz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2savwxsij.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2fljbqimx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2qsvmdzfq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2iirrfeyd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2mhiyvocu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cokffdlt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2rlyeokkr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2frvmgffb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ipywjspx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ckkvcjuq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2umwfvtlz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2wceczyvn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2nlosvyte.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2uxqjntbe.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2lgjpaaws.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bnsxhccc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ltoiqcwm.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rgvaumii.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ngreshwv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2awdtrdpa.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2odceesed.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2csognosk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2segcclpg.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kjeaeznd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pcmbebrc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2megujnnq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2glviisdz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2plzegebv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fkurwcgk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eplkrjze.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wyyvhqdo.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2hlxgrhfm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2szrgijks.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2shyyvxgr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2nnahiaqz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2znigiees.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2jhjvopeb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2rzkxpczq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2tgebfaxk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2hxvsdbjf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2wllqwqup.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2rdsfichk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2fbgptpzc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2prqyzjan.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lapecivp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kuksxmln.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2rrjyvdhq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vjirqjit.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fjpwwshm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2hfztlrur.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dbxokeop.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pvrsgtzb.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lrveixzc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lwzonyxq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vtwezxui.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2eeswawpe.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gvjopuje.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2kwyktejc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ncmlnuuf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2klvopgkf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pmmdsuhi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qqirhmtc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dmbpvbom.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2nvzamjpd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qilfyhkn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uldubapr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vucfnvnl.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2zkfsyxfc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pfapdkov.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2silgkogy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aggweenc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ctzenkji.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tsuglcin.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2enszhqhb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2shjmvood.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2uryifjlh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2tkvzzhvn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2zziecqoo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2uxrftvcw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ekxkudke.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ymvnhltw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2dnqttyxg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2omvqdlgn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2shxfbmhg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2gvecoltm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xremaexe.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2uupmhevy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qkribhyw.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2knfchogy.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2finoipmq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cgqqsdpm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jdxhvjje.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2pvrfghgy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2pbbildgx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2cqyggkgx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bvfpokqs.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2bobujyhf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vaiowcqc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2awrtjexa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xncudcit.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsewgehg.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2wxvokwhb.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkolmpgi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2vdrheoir.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2fcvqclmu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xpwbhchp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2wgcuiovd.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mpaijouq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hclyurvq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pvetmziv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zjnyrypo.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2orhtpqud.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2posrvdsy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ixucnbso.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2howblbaq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2lvcfxnot.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fmwepxol.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vhxkwjuw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wfpngbrg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2btexzolo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ladcpsnm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ktxsrvzi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2iftzmpis.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2nobepxfv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2xaskciao.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2aenqmyfr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wuzmjzhf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nubmugrd.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wxdavpro.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwlvjrzs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2kglqfcae.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2npbeeebi.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvyzhmmw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ypbqwbgv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2timtsqma.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cdtybcjw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vhwajeuo.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ehfxclzj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2csnciduz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2kxxccapn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ramodabm.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ljbzkkph.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2zaydrabg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2lsctkyzb.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fbmoghix.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gwwpmqdq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dhyenpde.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tmxrfgdn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2skphnjcc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2gxtbksug.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mgjwxtmx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2hgbjnljr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2dpjwvvwr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2pwdqwndb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2rtimypdl.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2jsdtcfeb.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2oiqbeods.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2cibvscrd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2kepqharc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2umtotitf.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2wainklrk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ciopzzyi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2klkrlqiu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2pxmrxaci.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijivdkmh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljxksfco.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2zfistwsn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2tliyetcv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jottdtev.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2qvephkte.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ztovejng.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ubhlvlpq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2xssdlbcs.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2urfukqkq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2doflrnal.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2zfykgsal.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2roszpefb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2qrjnimqb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2otxmhgeu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2antqzdzj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmwcovae.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dnkqyslb.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjolzlmj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmulfban.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2odasqibc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2nhqrjdpm.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzzalmop.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mpxrwbow.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2sprzprqb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2itoipfjc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2elehiqxz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jmzkrhnz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lxngnsyn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gxbyhtpr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fqwppsdc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qivcuygh.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2jvjelwfi.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2qjjpdoav.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hpolmytz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2cnragsyn.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2msfkkfdq.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yweujosa.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2bmvqkozd.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2hgzvvwqu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2upglaynh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2larnqbft.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2pykqziwo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2wbvfqizq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2mtgqczdm.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2bpfwbpsi.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2evmekchf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2mvxrhfzt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2ilrsehxa.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2srvgbrmz.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2xjhovfea.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2edvkmwlb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ihilazhx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2epdrdntc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2gzdmesqx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2zqqhravf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2qytqlkri.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2dzyvksvc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ektglzmp.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2yaoaajxo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2nhyoqkse.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2zyosmuza.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ywrlsbtm.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jczpdnwg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2uwtczfzd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2jkrfphsi.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2gkpxbupe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2aaadiznw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ezpmakrn.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ikuohemf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvzidbug.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2slkywrxx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2zfxhpicy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kwywgcff.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mxwjbdjc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2pavksfic.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ikurkttc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2wjhtgaae.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ugmslyot.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2qfsjhprl.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2afpapyod.html


<!-- 参考信息 -->