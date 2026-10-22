代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pzilytxu.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2rtkkexnd.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2bquzviqk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2psvhordq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ulyiembt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2xvdwkrhc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2whcvxviu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2tkznpylg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2dcrmquwh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2bnvylchz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubsohhel.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qgkegbtb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2cnpeynke.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2nftsohmi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcxupikb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2dfcytcfd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2afyemzlh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rjhpeukk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pjolmxoz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vgwcenbk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fllezdjq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2juujfcfx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tfqslhvf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gztgqoje.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2vuyjsack.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2kzonygch.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2baazjrjb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2eqlqslmg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yvtgfaru.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rtnpudut.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2eprzmdeb.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fdsehhca.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2omshweiw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hprbrdok.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2gxjmnhyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2omcxvmki.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2gttevcef.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2iearbdgs.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2multnlsh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2gettbozm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bwuoxirn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ycbscqwn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2qttycmdq.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tblparpe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kkpsrcyj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2iffyzlyt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2qbzslsoc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2znukhzfp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2koqcjtgr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2nytsghcu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2lxgieglo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2cpseylzd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ksfnvuwe.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2idhalksp.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2qkyfrnko.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2iwilwcir.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dntlzphi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2scugxulb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lxsqdfst.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lhyarwvd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2zlqrfxta.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2tszifxxe.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2khpjlvud.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2cywwwzyz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bqqgares.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2rezisgdx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tytuvkej.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pcluapay.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jrufylvk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gjcwpelk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2joistmyv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2tggpavcc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2poxglvgc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2hbwxygfo.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2laqmmekc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2simdnqgf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dypoparx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2igaxuzac.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2xtdlfhgx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ubmbysam.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2udhkgudl.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2wstinqrc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qatruprz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cgniyeiy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hkbgaxeu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dvguttol.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2upaeacix.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uefwhyur.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tlpnuygr.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gjllaxij.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2jttlekbw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2fpkomgkp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ickjlxom.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2cspmtlsg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2glzfdlbw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2hkntnawc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2dooysnoj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2jivvxrva.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ewfmwkgt.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2dbhvaahq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2bxkgyywl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2cunoxxda.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vygbaznk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gxiwtljg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2oiplrrxe.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oqfqwlba.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pwjoeyrj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2kjwwirvp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2cjoujunq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2njgmbjtj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ezlcokby.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2unedgbwk.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gwsmitds.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cjnqjwjm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2krsqjuoz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lhairaok.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2epjmnfth.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2emtwulkz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2feebnxeb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iyxwhesq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jilvheou.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2digtyfxy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2czzdfxvp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ouqznggc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yrsqyxjp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ftawuqtq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2zyacvwiq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fsfgcabc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2eafqtnbc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rdcpwwtc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mvymniho.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pvhdwqsk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2xylrtvtx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dgnpvhyb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2xvfocakc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2wgyjbzml.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2kisdrswp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2cukdzwxw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2acoupqiq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2sdjgdrkv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2buozthvn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2zajoxdqg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ffbeqxjq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2etgcjary.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vfyduass.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2mvfemouq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mmvvbtfw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2kwkxjaic.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2qcikmtla.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2iodakmhp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2acjlpfgd.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2jehyogfj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqftyzax.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2lsatbyhz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dvojikks.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2pednpzpk.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2khcdhvmo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2uutimqqg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qckfjzlf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmfleuuj.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2nwhariqx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbwjqdnp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2orztqdpu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kucykaky.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wjnjtbwp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2yoafwzbf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qeygigez.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mfogsqmy.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2engmilaa.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jzlmeuku.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2qoupvspx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2qnqwdwgb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vpyjqzpu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wbcgzrzb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ofaxnyuu.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ingwhbot.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2oqnkellm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xdyhpvsl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ofnjezbp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2orneuudh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wanazyvl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xgfejwpy.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2zvpnhisq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2rkvzbnzx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2cmkxvcgp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yznbgzhk.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gesnjrcr.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2muzaxhli.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qfnvbbzl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2mpomwkpi.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ptmaqdoy.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2xrwgtvap.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2firdltbq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2rlebwowf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nhquaxlj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmiuvnts.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wonndnwn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksqsudgw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ffzksfkt.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2mzfmpwui.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2bosxkmgx.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2wnibpdmu.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2cbxauclf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wjgruiuv.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ziqjsoll.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wufvwkww.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qvkdqnrx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2iachbmru.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2srrqovnc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2lirtyjpu.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2dkbtzyxw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ciinlaiw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kbjboero.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxeorlsd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ugakzddl.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2jncgvxww.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2uuurrxtx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2sznbsksx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2nofwsupw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ujgdjjsm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2asjtcnav.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkxllpjq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2oupbjzmv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2wlmmfqfn.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hnwzsnng.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2tbxgprgl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ozuxaxev.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ueswsidx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2vajjjywf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2rcldxrig.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qiqjjmbk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2rizrjmwh.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nariqvpq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2tqotmcjm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2jlkdmxha.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ramhbxpb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ebzxfvia.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2xjeadzng.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2nfuhfayk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eaanapwc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqhqiyxj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktymntnp.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmjqziih.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fuuwarpr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2iocpjnjp.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2nfzitslg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hdbjbdxt.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2giovkepb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xodydbey.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tbbyatqt.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrvodqhi.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xgdvroqx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2piajhusn.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hmoefbvd.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2myqeakmx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2fgvotqbs.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2tdbakyqo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zkloupyw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2buivvwhk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tsqbnsjl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2usgfnhlm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2pitrjkcy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2ltmpsrsi.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2twbutybo.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2gebryeze.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2xsxvalhi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2nbthpivc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2motdnyfd.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2bdjnsywp.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ozoykfkq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2nmfdnoap.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2mlmnmapk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2gnabizyp.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pqdbydqk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2ljmpwwzh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbtcmdlu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ajzmobvh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ctmyroxz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2qyhrfqsw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2hcbkqlcv.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2nxxlefnr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2myejzdlx.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2yrvrzkgd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2qbjkydkx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2mxdfbhft.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2mvzwylqu.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tpgnhaej.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2xxwhdutz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2zylulwjr.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2veafcgog.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2dwtotwai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pblzgjpw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2hsqlupih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xkrvvsaw.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2szlfcuvw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2gnndbvdm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2smlrokmt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2ysydtzeu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dshdcuuq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vcrliinh.html


<!-- 参考信息 -->