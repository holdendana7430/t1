代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tzaldkex.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qftpmoaj.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qdujmpzt.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nwfgdwrc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2hrjadozw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2wupuswvr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2masqofjm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2rjdrvpkd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ppttmorm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2elowixlc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2bpmrlczb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vrzxhorp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2cevnsqlx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2evbvdoui.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2hbxvqsak.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2cztjfniz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2iecxugsu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oflokmge.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ojbjwskq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2viuiaxuu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2whlndkff.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2dqhilgvs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hbseynbg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ogqefghh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2aqmaioli.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lyumjtxk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2azsiaaaf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cvhcstfe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ndfdsoqm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bgoxjras.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2lasdotgk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fzbyslvt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xtxvknii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nuxgetwp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ovtxanos.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oyoqugzn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2nktqohmz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2kkrdhvct.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pzwbuoyh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2spvrwkwa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cjapmylv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lpeywoog.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2tsdeomda.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vpniwxuk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mhhwmdjf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2klxcatrd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2uyvwrlfb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2kinqkdhe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2yujwppgm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vucczmkn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2meordbac.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2llgweqwx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2mcwdnthi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2rljqowkb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2empwumts.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2byjnwozr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2plsuzbzb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jjdjkjeo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mcturrfl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2boxwrfwk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2nssjbeyj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2pshazgto.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rlmhaxgb.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2cixxjfqi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qgnpczot.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ouwlvdoj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yyqtjtjv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2mnrrgmtw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2imvrxmgl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vhlngxxj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2riecrpyx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2kcuycljz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tbmmvnxs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2xzayinkb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lvojhxpl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iuujpcnk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jwmloocs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yojyecor.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2qtvqrooo.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dejvsusf.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zkpzzcpa.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2smfwaypl.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wfzfdqxu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gxgawfco.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eqqpyqet.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dfswwkec.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wmmyposm.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jextbzrc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bdbxvwwu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gahzdouy.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ktmkpocp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ngciyajc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2fpohrdzu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2fwjcyuhz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2fdihpgma.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2vvooxrkw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2qcdeebqb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2wzkssrxf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2scnzsoum.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2vmbzviyc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2grxshkmm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2bfkszoiu.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2vwitukcd.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cqjpfgvh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wxkvjats.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mliwuoax.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2svzcntcs.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ypkersqz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2jhmtucsc.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uzjydupq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vgewdjzj.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zjupnbsv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hvhpggcb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xlobxnzu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ychluuzk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ygoqmhej.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2xxcknyiq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2lzbimzxw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jelctviv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dqszjzqh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ekahaudo.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xvqhvnem.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2hveqozje.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2buuzcogw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2btzrhzzh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xkvgmpqt.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2dffqvfus.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wgoldzzl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2axevoefq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xajdperi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lokzcuvu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gusqjzwm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2gwpnxdec.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qmsmknnf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2botuqsky.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2lfxgsmge.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ilrgiqkn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2yscyyklx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2txfgzdjp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2cmnqpbsb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2dujuinfh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2lvfwbucm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ayyabcib.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2fjcdwxhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fxgjosll.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2hxwxpcfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sasyqnue.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2wahfehgy.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ptvcmnlg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2zqbfrgbq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vybxpelm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2chwpbgri.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ulnpxgit.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2sithrsdw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2puorfieb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2txifvfrj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hpcovzfw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2yaoidugw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ljwjuhua.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvczdlhd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohwvaezl.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fgfxkxbz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2qcwjxgbt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jpnhuymc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcgnydoq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2adcthpda.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2gtydsfvw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xkqlmaem.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2igdsdoub.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2tlcmgsof.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2bqxewbfs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2omxsmpbk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2eackaycj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2asfhdwuo.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2fgbuxliq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2npdkikmp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2avuhxzsl.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mxipacnj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2iycvkxll.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wrzcporf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fnmqzult.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2tajocggi.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ygmyyzje.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2cyxaaaec.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2plkjmcof.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2umclciyt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfvslqmu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zftjgsll.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ityexcbb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2bqwfywzp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2farnjdcn.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jgxbuccu.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2inakfhdz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2hlhdrpqv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzoxxnqa.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2shapvflb.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fslrfdpb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xduixvxv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ofkgasqv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2jmcfswee.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2cqqgspvu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2hkmvtyzs.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2wwnmmxsg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2wrznsull.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yastsxmo.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gsisegtb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cbylemdv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2pqnhvqak.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2fvtpjtei.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dmhhuqgc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2amngfyvr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2fmyaesus.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqypxqbl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2gkxielgb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2fubadnbg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2aopspszs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2qplkvkgg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2asfgnoex.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uggbiiui.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2wznwkcgj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2zvizbuth.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2dodyxfdj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2hnpzejfo.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2necbcrri.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2omzlktnv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2zzqfvquf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2eahqfdmt.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqwyabpl.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ivcfqytk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2mfpitjqx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xsjkdmmr.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ucimmghv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2iunqqvsr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2gxqqarty.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2glbtdcxw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bpbdnqjy.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ymxuzujr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2aoyvirdw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2cpjvrucj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rkdqpijx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2mlhssfrz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2luydgebv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2victigsp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wcnxsfvp.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2lxmfzvgb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2hrrhbbif.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2pcvsjsid.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qxjabwfb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2osrivhvv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wvqvzldo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wsfdjkaj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rhsqaqai.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ogtyvpyy.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vqvoaftn.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vfjbkawn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2hjaqxrcs.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2xehcgkrm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gpplptrv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ilzizwof.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wotdtcng.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tyfohvdt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2btheebyh.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2xzrwrqvw.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2vhqqdvjw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2rfpvulyd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2auedazwx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2kfynjjzw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2bcmsejtd.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2tuyonjwo.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wsjydswk.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2yenewtsw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2vghmsljo.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2sikvyipu.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gjtaaotm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2oqzhzlhv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2egnsfvqz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2iikxxyqt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2otxlobfd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2dnuylqva.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2fupdbobc.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2rbmajvqz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2gztygrzi.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2yldpgcsw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2legylnjf.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2rjemidaz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2eufispjp.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xyvwgoqu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2rayitovy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2shpbsqcp.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2wklwbqzf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2cdfofejw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2drtfwvos.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2kaplbixw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hhmhdugv.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2oirhurqj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hawutbrr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2pcydclfl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2sndrkpuk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2bozbozfc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ultlulxs.html


<!-- 参考信息 -->