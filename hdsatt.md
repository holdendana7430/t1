代发 wailian999

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2okfbqzvs.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2qeouinwn.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2gdlozgwe.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2kkldmibm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2wbtkhffy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfvfgebt.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2fclrsxkr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jguvdhui.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ehxoekja.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2fjiowjlu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrimdnjt.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2xpbdinsa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2gfeevlaq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ihrcikzy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tpxxafnh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bmuvtuhs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fxmhtrya.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2xmbbjxgg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qwfrkcmw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pqnyvatx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2nuiensct.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ukzakfna.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yosfgimm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2euktijib.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cxbytcbc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2smtjapio.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2gmlvvvam.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cxofpzxy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vghgocbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eniagqfj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2wjwnlvcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vejxadkm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wthbpzjs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2egqaflwv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mdrxlekl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2xoqxzbie.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2awglkmim.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2iphpjwjc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2bokhsmgf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lwtulbqc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ugeioxtn.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2vncmzqno.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ixqdzfhn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2dhoezgdy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2meytqoxb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkshlyrc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tpbijgwy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2mjkchnkn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2csrzokvz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2mhporsvb.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2tienulaz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jxebmamx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2cyiorbas.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wcdvvesa.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vwszixjr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2zvmwmjjz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2cnznpqkv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2phsgyspi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jzwprblj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2qppotqul.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wzjlovlg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2lzslsgkb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qpajrihj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vogierpp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2lrjukzyu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sijbknwj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2chidxrnz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2csdgyarc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2zihpvyow.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xvmyjrvj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gqqmcvsy.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xfrnewai.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kqonjplf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rhsynzqc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2focfwyjl.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dvtinyrr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rzyvfrox.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ifatnjxa.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vvlhcyfq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nhthxtka.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cmebqjba.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nvkqiobo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2asoagfcy.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aqiyrmnz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ufzowkyp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ygkwqfrk.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2vcgvhvxp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eadrygic.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gbfybvtt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vxmaqnhd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2pvzioyio.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2pdbzcrul.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2zpcexlsw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2grsnqrja.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2cxhtotix.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2cqaounog.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2dqxjnsrf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2wirpovmj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sxdoatcl.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vswxrrcf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2rngfybga.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lqeptxul.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mlxhhtwr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cwjjsqqy.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2woevayor.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hpofubwc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fkggyebh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tzgyqnyw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2iwuntegf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2outfjqdi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2dihybjuh.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2foxmwbdg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2sdjcfrct.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2aqrxrtkz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fdgkmetm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yqvperuj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rgkefqfo.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oedylwjv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2eppniekj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hxdgefsy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oypstdqa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sqceteec.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2uefdobpf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rbxjtwls.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jlohwijq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kcpesrrf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tsutelki.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2krjspanm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2avjunwcu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wvetfxin.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2iwnyngpo.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2atsepujn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2yguqogvt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2rptoxdvo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2qzgkvekx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jhbvixdp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ilizkhpy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2khjpmaec.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2zyjxckqy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ecbomjwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xyirfgiu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2csuifnxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ttpytolf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2mufhrvxh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2qhudwenx.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ixtbfrlx.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wndfmgee.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2lpnyfsjj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2lnqmhmzq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2wvmeflta.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2wfauzwmg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rrxjtxsj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2eioxtxig.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2xbgrjggq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2hkdvecju.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzwddvwk.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2nzqoaokd.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vklfcxzf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2abwkzclz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2bigzlkgi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwgxwlzr.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2xsvzsveo.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qhjbldhh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dyqbrukj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2israygff.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2dmvkgnzk.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2eqafghbr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2soobtivh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2yjegamqk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2oxqdbydg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ffmfjayy.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2muhwxgrk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ttkvmvws.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcytjfza.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkhsicur.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yiqabcch.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yckfjwvt.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zfdisgzl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mvwzmkcb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2xsoflvyj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2kooaxzdh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dfpkbhdl.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvrlqcut.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xyklvcjl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vyexuamc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2eptvvjqm.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2uhnogfpb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gtvhsozp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2mirfvqjq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2movxnrgx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zlsqfzvg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ztvkymlk.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2touziygw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kxrigzbt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2hvttlqqj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2dwqtavjv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2tgunbbxr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2nucdvtxn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2vctzqgvs.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pjyspmzr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mjzsjmbd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qiztbeho.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wzxfuhyi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2dqbhchwo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2bpsxtwgl.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wbdzzwyo.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2zwsrsunw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2yvptatuw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2etoqhifg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2bqoxjqql.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2zuyqqcga.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kiuayqmv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2eufdhwed.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2mmdhkexz.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2nfnfvgvk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2finufdnz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ejhlgecl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2rztcvqwu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2tipseyyn.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2tjezfwaf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2svmoqmph.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2taduqbfq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2dxkolilo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2bpspwohl.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2xqzasdno.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2kcphihqw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2azenthsv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2gjiwthfo.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2headbann.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2oesxmcjc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2pptigrgv.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2pfnumkph.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2czltparr.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2bcepqjza.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ozhfaoax.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2czmvlnlm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkoncpbo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ggjczhye.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2clfgfsep.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lnelnudy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2yzyjaswv.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2zerdqioi.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2vnfpfjrk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xstjbegj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dyfkwoor.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2suwbjfqy.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jgvjfrqr.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrehwkts.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ekgkgbfq.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2iiacmuvv.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2occdlnid.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2cbolfbjy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2xtgwngtt.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dxtilobf.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yuvjonhs.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fpspxiuv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2aiwccpjm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2wzgolexi.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ovqtycsu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2lfghvkld.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2flkqvssc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2mwzabphl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2xkywugxz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2zlhecqbg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2fcweenkq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2wjnpgsyc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2yyoiubxl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2emqbacha.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2jdfxkqld.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2yyezzgku.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2mwjdjcrf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2luzjbrrr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2dxvaavvz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yihrbggx.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2hkyfoudk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2pmczzuxh.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ipgbtmlr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2obxzknhy.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2brorktpz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2nflvpedw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2grllxoxt.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zwhljyxq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ccmypgnj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2tbefuioc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ctaofyfe.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2wvvqvtif.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2bflhnnck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwqrmhjq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2nhvkncut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yolbzqpn.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2mugcnskq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2efaswhhb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2qcjdnezr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jtqmyest.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yqfvueci.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwabohtm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2freekpuo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2mgzlyjbu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2xinjvttj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2nvcqcffo.html


<!-- 参考信息 -->