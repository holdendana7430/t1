代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jfgfixww.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2badhyllp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dqyyervy.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2dnhpwqzf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2rzhzwrpq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2tvlrqqtg.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2zuiymmal.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2mqlnsbbr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2gqkrhrui.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oaybxxga.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2rqluqjcq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2niikuxxw.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmgzgdmd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2vncncjda.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2msewvqcd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2wnkindbl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2dznvsery.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lsqupzfv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sxxyvugi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dvoylmuw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wlfgvlck.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2itkwniuh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tzmapzho.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ptggzvht.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2khnoivxd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2pyreihpz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qktyunbt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2slfhtfmj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2eymfhxfn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2cbmwtxxu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2cdwlpcfd.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vxltljdl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vxyzypzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2neeuswxu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ieigdypq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2idwuetlq.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xdkftzsy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2dclcenxy.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oftsdakq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ffqwcumf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2daufnfol.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hfdrzbxx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ecvtpdlp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tdkerdqx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pcummwib.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2sdzcxgsx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2fhjkhhlg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygsqudqy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rbvtwuju.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2byqsxqrc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2khrkuddq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2znczcvrj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2jmsuqeuc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2qabxafoi.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2emiotjkn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mmprxxhm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vuapsils.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cqnbjyom.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zlygifhg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2nwdtfvse.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2miqibsln.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2qhflnwqj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fpchigan.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2jayrpuwq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2bplubqoo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2xoovamab.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sgogbgfb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rdtdktqr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2mczaorhj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ijijejzb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2rxfgzfvt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2zbgllrrg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2kdarvyvm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2dyjzcwhh.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oiwrywvk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gqtmijwq.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hkuqwebv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2evhcnjdh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2upkxsdcm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pqicdiwk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rqswfbcs.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2zkufsbis.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2alkougck.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uyahkeyq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yrlgbvyf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bybdalbn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xmavaejz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ekvrmart.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gdqhxjqt.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zkkesqmo.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2aigxtdpq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ybhvdwri.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tkrsittq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2gvtrqupa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ufbpjgjn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2tzqzxbft.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2qgzombmc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2dmpyfxoc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2lvlobzqw.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2eurpvzea.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xpvfwmli.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ajzqosmt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ccwghacq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dbbcnmtu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2cscthgac.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2twrvdqyl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jpjhqmqb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cigjlljz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2xxegjvoo.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jghrwtmj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ucvdvhmf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mkfpkifc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hxjvinav.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pnonatuw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2sbgwgxgh.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2llyswzfd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2gpzhwfhk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2paggwjyb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mftbqqou.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ywjhblkz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zcoivqoh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sdmaiozw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ramplomk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2igqleztp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zcdqsegp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dspidpwa.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2kpblzfgw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jqstrrfn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lomwnlew.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2crqelbqk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dmehwuvi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gblofbor.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2nofsymgc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2obtyufmy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2nmxulyzs.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2vcdrehbg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2udlfaeyv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2vllljory.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2gygogaqr.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ppinwqiz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2zmjyasux.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2vyrhovsm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2spmcizxv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2mizzzugd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mzudsqxj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2kbrrzxgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gsfiiqju.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2sgkmhpxp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2xpedzovg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2dmojmyel.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rgcsseox.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2cmygdttw.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qovlpkav.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ffubskmv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2xqwqghlt.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kcagmpqo.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2aknmqysj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ivptkqja.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzkuieyt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2uxeupjrr.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2gkcusnxo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yypgwbbz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2feojgtbo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ehxqurfb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2icttumgt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2rrybjoqb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2pkdtnnny.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ysjwgmsx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2onxwoqji.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2kneuprop.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2jzgofist.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2waqhdnmv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2leeuxuwu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mszqrmgi.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2nzfjnled.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2crxbkawl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vigxwylq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2abwrnzts.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gubdhntp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dywvejrv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bztozvzi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ithacwoj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gkcimncj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2oqfjojqx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2kspnpbzy.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ljdholaj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtdehbfa.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pldwvgkw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yfewtpix.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2smgjjwct.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2kzcnvbjk.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2qljaodfa.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2jneikxgy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ubgqzhpc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwyqboih.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnfsksfr.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2klnastlc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dbhssnkj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ecwghpjh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2qhrrhbta.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ujanyszm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2xjqlxtwk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2dwmtzclw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ogdrgioi.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wqdhtghj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kcrqpbeo.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wdadkvku.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2xazfsjpf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2awadzcsb.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fsifqysh.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2pppgikhb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2doijqtol.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2feezoaif.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bpejeyfk.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2bihcrger.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2djukgkjr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2aofmhezi.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2izgeffrc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2owtwwdww.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2pdxnjwvx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2gtqngrvl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2lkyegryf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2abvdfdrw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2yioxtone.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2rvtwnpgd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2rubyzknf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2hdumoipi.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2esvlkgml.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2lykpdilo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2exnsjzpd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hdugsmec.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2kwmiobyg.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xpwhgrju.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2qewpmaru.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2lskcdwxp.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ahtrhkvk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ficfztwx.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ngzdwqdr.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2flmjaydq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pbztoppt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2htcbmiya.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fsqhxvor.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2axubqusw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2btvglcrr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2cuyuzean.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2aovwegjf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2byocleqa.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2osggdcbh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rymmopjz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aduwypxq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2psiavjks.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmfrqhly.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fkqugpep.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zswutfza.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2zcmjpjfx.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2fbohejjh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2nssugujd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2npqtqftk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2nlwoupmo.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uhryrzsn.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hbmiddlc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2qtksrlac.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2zxnbbjgv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2xhebjsrz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2fucvqzwc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2dgwewjax.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2zhmibnbu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2eymslepq.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2cfxehgsn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvlygmfo.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2lpdzkwwt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2dskdbvfq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2vlnwsstk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2vwoigbwv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2hhcxfhhk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2anjeceqi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2gbgwctdj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yqafufdn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2gpdkgtgt.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2sdldxnmm.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2chwyfvta.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ythciiqg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2hpumvque.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2hfuzgjmu.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2mojrtiuq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wlgfglaw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2rzjgwezl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2rebtbmfk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2xsqwlbqb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2gwvhpjnc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2qwlseiyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sjwpeigi.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2eakedatd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfhpferi.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2huiqwdsc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2pcpwddre.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2srulozal.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2exubapzw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2avnvbixh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2uzxsjfoj.html


<!-- 参考信息 -->